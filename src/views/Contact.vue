<template>
  <v-container>
    <v-layout row align-center>
      <v-flex>
        <h1 class="display-1">Contact</h1>
        <p>Send us a message and we will get back to you within 24 hours.</p>
        <!-- <ContactForm /> -->
        <ContactFormTypeForm />
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  // import ContactForm from '@/components/ContactForm'
  import ContactFormTypeForm from '@/components/ContactFormTypeForm'

  export default {
    components: {
      // ContactForm
      ContactFormTypeForm
    }
  }
</script>
