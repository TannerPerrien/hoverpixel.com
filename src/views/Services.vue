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
          { key: 'real-estate', name: 'Real Estate', summary: 'We all know how important high quality photos are when it comes to marketing real estate, but are you missing a higher perspective?  We can provide you with high resolution, highly detailed aerial photography for your listings that will separate you from the rest of the pack.  Packages start at $99.' },
          { key: 'utilities', name: 'Utilities', summary: 'The days of climbing ladders to inspect towers visually or with the aid of instrumentation are over.  Our fleet of unmanned aircraft can get there, view and record, and move on before a human would have time to don the required safety gear.  We can provide high resolution imagry or thermal imagery to give you the data you need.' },
          { key: 'construction', name: 'Construction', summary: 'From aerial site surveys to code inspections to documenting for posterity, being able to capture imagery from above is a necessity.  Allow us to capture these images at a fraction of the cost and imposition of hiring other aerial photography and inspection such has helicopters or climbers.' },
          { key: 'civil-engineering', name: 'Civil Engineering', summary: 'Drones are able to capture top down imagery or get a vantage point that is not easily achieved by ground photography.  Drone videography can be helpful in studying anything from traffic patterns to wildlife activity.' },
          { key: 'cinematography', name: 'Cinematography', summary: 'Add aerial video to your existing footage OR have us shoot an entire project.  Our footage is compelling, silky smooth, and produced at 4K resolution!' },
          { key: 'consulting', name: 'Consulting', summary: 'Do you want to fly your own drone or take a test flight with one of ours?  Would you like some guidance on FAA regulation when it comes to air space or protocol?  We are here for you!' },
        ]
      }
    }
  }
</script>
