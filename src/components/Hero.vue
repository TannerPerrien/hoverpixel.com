<template>
  <v-parallax height="700" :src="require('@/assets/hero.png')">
    <v-container fluid>
      <v-layout row fill-height align-end justify-center>
        <v-flex shrink>
          <v-layout column mb-5>
            <v-layout row align-center wrap>
              <v-flex tag="h1" class="display-3">FAA Approved</v-flex>
              <v-flex>
                <v-btn to="/contact" dark large color="red">Contact</v-btn>
              </v-flex>
            </v-layout>
            <v-flex shrink tag="h4" class="title hidden-sm-and-down">Real-estate - Utilities - Construction - Civil Engineering - Cinematography - Consulting</v-flex>
            <v-flex shrink tag="h4" class="title hidden-md-and-up">
              <ul>
                <li>Real-estate</li>
                <li>Utilities</li>
                <li>Construction</li>
                <li>Civil Engineering</li>
                <li>Cinematography</li>
                <li>Consulting</li>
              </ul>
            </v-flex>
          </v-layout>
        </v-flex>
      </v-layout>
    </v-container>
  </v-parallax>
</template>
