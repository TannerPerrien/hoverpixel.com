<template>
  <v-card class="card">
    <div class="pa-3">
      <h4 class="display-2">{{ title }}</h4>
      <p class="subheading">{{ subtitle }}</p>
      <p class="body-2">
        <slot />
      </p>
    </div>
  </v-card>
</template>

<script>
  export default {
    props: {
      title: String,
      subtitle: String
    },
    data: function () {
      return {
        counter: this.title,
        subtitle: this.subtitle
      }
    }
  }
</script>

<style scoped>
.card {
  opacity: 0.7;
}
</style>
