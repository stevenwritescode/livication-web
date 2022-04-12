<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex flex-sm-shrink-0 align-left">
        <v-img
          :src="require('@/assets/Livication_Logo_NoTagline_Light.svg')"
          class="my-3"
          contain
          fill="white"
          max-height="30"
          max-width="150"
          position="left"
        />
      </div>

      <v-spacer></v-spacer>
      <v-btn
        class="d-flex"
        href="https://discord.gg/sjtNgQvJAU"
        target="_blank"
        text
        icon
      >
        <v-icon>mdi-discord</v-icon>
      </v-btn>
      <v-btn
        href="mailto:info@livication.com"
        target="_blank"
        text
        icon
        class="d-flex"
      >
        <v-icon>mdi-email</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'App',

  data: () => ({
    //
  })
})
</script>
