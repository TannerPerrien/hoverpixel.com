<template>
  <v-container fluid>
    <v-layout row align-center>
      <v-flex>
        <h1 class="display-1">Services</h1>
        <v-timeline dense>
          <v-timeline-item
            v-for="service in services"
            v-bind:key="service.key">
            <template v-slot:icon>
              <v-avatar>
                <img :src="require('@/assets/services-icon-' + service.key + '.png')">
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline">{{ service.name }}</v-card-title>
              <v-card-text>{{ service.summary }}</v-card-text>
            </v-card>
          </v-timeline-item>
        </v-timeline>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data: function() {
      return {
        services: [
          { key: 'real-estate', name: 'Real Estate', summary: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.' },
          { key: 'utilities', name: 'Utilities', summary: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.' },
          { key: 'construction', name: 'Construction', summary: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.' },
          { key: 'civil-engineering', name: 'Civil Engineering', summary: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.' },
          { key: 'cinematography', name: 'Cinematography', summary: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.' },
          { key: 'consulting', name: 'Consulting', summary: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.' },
        ]
      }
    }
  }
</script>
