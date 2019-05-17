<template>
  <v-parallax height="700" :src="require('@/assets/hero.png')">
    <v-container fluid>
      <v-layout row fill-height align-end justify-center>
        <v-flex shrink>
          <v-layout column mb-5>
            <v-layout row align-center>
              <v-flex tag="h1" class="display-3">FAA Approved</v-flex>
              <v-flex ml-5>
                <v-btn to="/contact" dark large color="red">Contact</v-btn>
              </v-flex>
            </v-layout>
            <v-flex shrink tag="h4" class="title">Real-estate - Utilities - Construction - Civil Engineering - Cinematography - Consulting</v-flex>
          </v-layout>
        </v-flex>
      </v-layout>
    </v-container>
  </v-parallax>
</template>
