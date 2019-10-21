<template>
  <v-container grid-list-lg>
    <v-layout row>
      <v-flex xs12 class="text-xs-center display-1 font-weight-black my-5"
        >What I can help with</v-flex
      >
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
export default {
  name: "HomeSkills",
  data() {
    return {
      skills: [
        {
          name: "Prototyping",
          description: "Wireframe to reality. Proficient in Adobe Photoshop and XD. I have experience creating high fidelity prototypes rapidly and as well as diligently and informed by user feedback. Balsamique also. Pen and paper prototypes is the old reliable"
        },
        {
          name: "User Interface",
          description: "My specialty for 5+ years. Every aspect relating to the DOM. From creating static Photoshop files to implementing as robust, scalable solutions with an emphasis on user experience"
        },
        {
          name: "Javascript",
          description: "Angular js and Angular for 5 years. Experience with Vue js, stencil js, react, backbone js, all versions of Bootstrap, Google material, bulma, jQuery and plenty of vanilla JS"
        },
        {
          name: "Design Thinking",
          description: "Founder of the Accenture Design thinking guild. Monthly presentations and spreading the good work. Bringing Dt into all projects. Presenter at the design thinking academy workshops"
        },
        {
          name: "Optimization",
          description: "Always been fascinated with improving performance where possible in the web, especially the quick-win changes that have big impact and small overhead."
        },
        {
          name: "Search Engine Optimization",
          description: "Founder of simplecss.eu. a pet project that gained popularity, yielded ad revenue and sold for profit. Storing domain authority highly ranked in Google search results."
        },
        {
          name: "Responsive Web Design",
          description: "Using bootstrap since it was in its infancy. I lean toward as mobile first approach and an efficient use of space. Experience with bulma, foundation aswell as flexbox, CSS grid and angular flex layout"
        },
        {
          name: "Mobile Development",
          description: "Extremely enthusiastic about ionic and integrating with other js frameworks angular, react etc. Ionic, angular and stencil. Built a number of applications using ionic. As a front end engineer I lean towards this approach but have also built apps using native Java and XML for Android, the good old fashioned way!"
        },
        {
          name: "Wordpress",
          description: "Extensive experience with WordPress websites using themes, customizing themes, from scratch, for blogs, for sites. This my staple CMS"
        },
        {
          name: "Identity",
          description: "Logo creation, custom websites, blogs, graphic design, branding guidelines, colour palettes, consistency. Created identities for small projects to large scale organisations."
        },
        {
          name: "Workflow",
          description: "Agile - Scrum, Git flow, BEM"
        },
        {
          name: "Services",
          description: "Experience writing custom services leveraging 3rd party APIs, consuming response and parsing into human readable format only he UI."
        },
        {
          name: "Accessibility",
          description: "Pa11y, wave, screen reader, Google lighthouse audits"
        }
      ]
    };
  }
};
</script>

<style scoped></style>
