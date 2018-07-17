<template>
  <v-app>
    <v-toolbar class="secondary">
      <v-toolbar-side-icon class="hidden-md-and-up" @click.stop="drawer = !drawer">
        
        
      
      </v-toolbar-side-icon>
      <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
    >
      <v-list class="pa-1">
      </v-list>

      <v-list class="pt-0" dense>
        <v-divider></v-divider>

        <v-list-tile
          v-for="item in items"
          :key="item.title"
          @click=" "
        >
          <!-- <v-list-tile-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-tile-action> -->

          <v-list-tile-content>
            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
 
      
      <v-toolbar-title>JAFFA AHARONOV</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        
        <v-btn flat :to="{name: 'Projects'}">
         <span>PROJECTS</span>
          </v-btn>
        
        <v-btn flat>ABOUT</v-btn>
        <v-btn flat>Link Three</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-content class="primary">
      <router-view/>
    </v-content>
    <v-footer :fixed="fixed" app class="secondary">
      <span>&copy; 2018 jaffa aharonov</span>
    </v-footer>
  </v-app>
</template>
<style>

/* .landing-image-div {
    height: 450px;
    width: 675px;
    overflow: hidden;
    border-radius: 50%;
} */
.landing-image-div img {
  
    overflow: hidden;
    border-radius: 50%;
   width: 50%;
  height: auto;
  -webkit-clip-path: polygon(44% 0, 1% 24%, 30% 100%, 93% 68%, 91% 8%);
clip-path: polygon(44% 0, 1% 24%, 30% 100%, 93% 68%, 91% 8%);

}

.text {
  padding-left: 25%;
  padding-right: 25%;
  text-align: center;
}

</style>
<script>
export default {
  data () {
    return {
      drawer: null,
      items: [
          { title: 'Projects', icon: 'dashboard' },
          { title: 'About', icon: 'question_answer' }
      ]
    }
  },
  name: 'App'
}
</script>
