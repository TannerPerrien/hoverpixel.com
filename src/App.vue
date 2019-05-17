<template>
  <v-app>
    <v-toolbar app dark color="#515151" height="100">
      <v-toolbar-title class="headline text-uppercase">
        <router-link to="/">
          <v-img
            :src="require('./assets/logo.svg')"
            class="my-3"
            contain
            width="463"
            height="70"
            />
      </router-link>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <!-- <v-btn
        flat
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
      > -->
        <!-- <span class="mr-2">Latest Release</span> -->
      <!-- </v-btn> -->
      <v-toolbar-items>
        <v-btn flat to="/services">Services</v-btn>
        <v-btn flat to="/about">About</v-btn>
        <v-btn flat to="/contact">Contact</v-btn>
      </v-toolbar-items>
    </v-toolbar>

    <v-content>
      <router-view/>
    </v-content>
  </v-app>
</template>
