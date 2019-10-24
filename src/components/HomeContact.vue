<template>
  <v-container>
    <v-layout row>
      <v-flex xs12 class="text-xs-center display-1 font-weight-black my-5">Contact</v-flex>
    </v-layout>
    <v-layout row>
      <v-flex 
        xs12 sm12 md6 
        v-for="contact in contacts" 
        v-bind:key="contact"
      >
        <div class="headline mt-3">
          {{contact.name}}
          <i class="material-icons">
            {{contact.icon}}
          </i>
        </div>
        <p class="subheading mt-3">
          <a 
            target="_blank" 
            v-bind:href="contact.link" 
            v-bind:key="contact"
          >
            {{contact.text}}
          </a>
        </p>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import Contacts from '../assets/data/contacts-section/contacts.json'

export default {
  name: "HomeContact",
    data() {
    return {
      contacts: Contacts
    };
  }
};
</script>

<style scoped></style>
