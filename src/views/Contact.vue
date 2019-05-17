<template>
  <v-container>
    <v-layout row align-center>
      <v-flex>
        <h1 class="display-1">Contact</h1>
        <p>Send us a message and we will get back to you within 24 hours.</p>
        <ContactForm />
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  import ContactForm from '@/components/ContactForm'

  export default {
    components: {
      ContactForm
    }
  }
</script>
