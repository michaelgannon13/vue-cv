<template>
  <v-toolbar>
    <v-toolbar-title>Michael Gannon</v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items>
      <a href="#details" class="button">
        <v-btn text>
          <v-icon>account_circle</v-icon>
          About Me
        </v-btn>
      </a>
      <a href="#skills" class="button">
        <v-btn text>
          <v-icon>build</v-icon>
          What I can Do
        </v-btn>
      </a>
      <a href="#contact" class="button">
        <v-btn text>
          <v-icon>email</v-icon>
          Contact
        </v-btn>
      </a>
    </v-toolbar-items>
  </v-toolbar>
</template>

<script>
export default {
  name: "AppNavigation"
};
</script>

<style scoped>
  a.button {
    text-decoration: none;
    margin: auto;
  }
</style>
