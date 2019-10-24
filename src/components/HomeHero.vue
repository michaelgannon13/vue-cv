<template>
  <v-container fluid fill-height class="home-hero">
    <v-layout justify-center align-center column pa-5>
      <div class="display-4 font-weight-black white--text text-xs-center">
        FRONT-END
      </div>
      <div class="display-4 font-weight-black white--text text-xs-center mb-3">
        CONSULTANT
      </div>
      <div class="display-1 font-weight-bold white--text text-xs-center">
        Michael Gannon
      </div>
      <v-btn fab class="mt-5 brown darken-4">
        <v-icon large color="white">expand_more</v-icon>
      </v-btn>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "HomeHero"
};
</script>

<style scoped>
.home-hero {
  background: url("./../assets/deveoper-stock.jpg");
  background-size: cover;
  width: 100%;
  height: 100%;
  max-height: 100vh;
  filter: hue-rotate(50deg);
}
</style>
