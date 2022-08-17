<template>
  <v-app dark>
    <!-- Navigation Bar -->
    <v-app-bar hide-on-scroll elevation=0 app class="nav-bar">
      <v-btn text @click="scroll('Abouts')">About</v-btn>
      <v-btn text @click="scroll('Skill')">Skills</v-btn>
      <!-- <v-btn class="d-none d-sm-flex" text>Portfolio</v-btn> -->
      <v-btn text @click="scroll('foot')">Contact</v-btn>
      <!-- class="d-none d-sm-flex" -->
      <!-- <v-app-bar-nav-icon class="menu d-flex d-sm-none " @click.stop="drawer =!drawer"></v-app-bar-nav-icon> -->
    </v-app-bar>

  <!-- <v-navigation-drawer clipped v-model="drawer" absolute temporary>
    <v-list>
      <v-list-item-group v-model="selectedItem">
        <v-list-item v-for="(item,i) in items" :key="i">
          <v-list-item-content>
            <v-list-item-title v-text="item.text"></v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list-item-group>
    </v-list>

  </v-navigation-drawer> -->

    <!-- Main Page/ Screen -->
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
      <v-container>
        <About id="Abouts"/>
      </v-container>
      <v-container>
        <Skill id="Skill"/>
      </v-container>
    </v-main>
    <!-- Footer/Contacts -->
    <v-footer id="foot">
      <contact/>
    </v-footer>
  </v-app>
</template>

<script>
import About from '../pages/about.vue'
import contact from '../pages/contact.vue'
import Skill from '../pages/skill.vue'
export default {
  components: { contact, About, Skill },
  name: 'DefaultLayout',
  data() {
    return {
      drawer: false,
      selectedItem: 0,
      items: [
        { text: 'About'},
        { text: 'Skills'},
        { text: 'Contact'},
      ],
    }
  },
  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Abel&family=Jost&family=Poppins:wght@200;400&display=swap');
.v-toolbar__content{
  justify-content: center;
  background: #2D2D2D;
}
.v-main__wrap{
  background: #2D2D2D;
  margin: 0;
}
.v-btn{
  font-family: 'Jost', sans-serif;
}
.v-sheet.v-footer{
  background: #414141;
}
.menu{
  position: absolute;
  right: 0;
}
.v-application--is-ltr .v-toolbar__content > .v-btn.v-btn--icon:last-child, .v-application--is-ltr .v-toolbar__extension > .v-btn.v-btn--icon:last-child{
  margin-right: 10px;
}
.v-main{
  padding: 0px; 
}
*{
  font-family: 'Jost', sans-serif;
  color: white;
}
</style>
