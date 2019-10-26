<template>
  <v-toolbar>
    <v-toolbar-title>Michael Gannon</v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items>
      <v-btn text>
        <v-icon>account_circle</v-icon>
        About Me
      </v-btn>
      <v-btn text>
        <v-icon>build</v-icon>
        What I can Do
      </v-btn>
      <v-btn text>
        <v-icon>email</v-icon>
        Contact
      </v-btn>
    </v-toolbar-items>
  </v-toolbar>
</template>

<script>
export default {
  name: "AppNavigation"
};
</script>

<style scoped></style>
