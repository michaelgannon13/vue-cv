<template>
  <v-container grid-list-lg>
    <v-layout row>
      <v-flex xs12 class="text-xs-center display-1 font-weight-black my-5">What I can do for you</v-flex>
    </v-layout>
    <v-layout row wrap>
      <v-flex xs12 sm12 md4 v-for="skill in skills" v-bind:key="skill">
        <v-card>
          <v-img src="http://source.unsplash.com/hjCA3ecCXAQ" height="500px">
            <v-container fill-height fluid>
              <v-layout fill-height>
                <v-flex xs12 align-end flexbox>
                  <span class="headline white--text">{{ skill.name }}</span>
                </v-flex>
              </v-layout>
            </v-container>
          </v-img>

          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">{{ skill.name }}</h3>
              <div>
                {{ skill.description }}
              </div>
            </div>
          </v-card-title>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import Skills from '../assets/data/skills.json'

export default {
  name: "HomeSkills",
  data() {
    return {
      skills: Skills
    };
  }
};
</script>

<style scoped></style>
