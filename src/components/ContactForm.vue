<!-- https://mailthis.to/ -->
<template>
  <!-- class="mx-auto"
    style="max-width: 500px;" -->
  <v-card>
    <v-form class="pa-3">
      <v-text-field
        v-model="name"
        color="red"
        v-validate="'required'"
        :error-messages="errors.collect('name')"
        label="Name"
        data-vv-name="name"
        required
      />
      <v-text-field
        v-model="email"
        color="red"
        v-validate="'required|email'"
        :error-messages="errors.collect('email')"
        label="E-mail"
        data-vv-name="email"
        required
      />
      <v-textarea
        v-model="message"
        auto-grow
        color="red"
        rows="1"
        v-validate="'required'"
        :error-messages="errors.collect('message')"
        label="Message"
        data-vv-name="message"
        required
      />
    </v-form>
    <v-divider></v-divider>
    <v-card-actions>
      <v-spacer></v-spacer>
      <v-btn
        class="white--text"
        color="red accent-4"
        @click="submit"
        >
        Submit
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
  import axios  from 'axios'

  export default {
    $_veeValidate: {
      validator: 'new'
    },

    data: () => ({
      name: '',
      email: '',
      message: ''
    }),

    mounted () {
      this.$validator.localize('en', this.dictionary)
    },

    methods: {
      submit () {
        if (this.$validator.validateAll()) {
          axios.post('https://mailthis.to/hello@hoverpixel.com', {
            _subject: 'Message from HoverPixel',
            name: this.name,
            email: this.email,
            message: this.message
          })
          .then(function (response) {
            location.href = 'https://mailthis.to/confirm'
          })
          .catch(function (error) {
            console.log(error);
          });
        }
      }
    }
  }
</script>