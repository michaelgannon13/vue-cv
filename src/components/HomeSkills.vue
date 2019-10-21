<template>
  <v-container grid-list-lg>
    <v-layout row>
      <v-flex xs12 class="text-xs-center display-1 font-weight-black my-5">What I can help with</v-flex>
    </v-layout>
    <v-layout row wrap>




      <v-flex xs12 sm12 md4 v-bind:key v-for="skill in skills">
        <v-card>
          <v-img src="http://source.unsplash.com/hjCA3ecCXAQ" height="500px">
            <v-container fill-height fluid>
              <v-layout fill-height>
                <v-flex xs12 align-end flexbox>
                  <span class="headline white--text">{{skill.name}}</span>
                </v-flex>
              </v-layout>
            </v-container>
          </v-img>

          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">{{skill.name}}</h3>
              <div>Wireframe to reality.
Proficient in Adobe Photoshop and XD. I've experience creating high fidelity prototypes rapidly and as well as diligently and informed by user feedback. Balsamique also. Pen and paper prototypes is the old reliable </div>
            </div>
          </v-card-title>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "HomeSkills",
    data() {
    return {
      skills: [
        { 
          name: 'Prototyping'
        }, 
        { 
          title: 'Javascript'
        }, 
        { 
          title: 'Responsive Web Design' 
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>