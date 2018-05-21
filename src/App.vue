<template>
  <v-app>
    <!-- <v-toolbar class="secondary">
      <v-toolbar-title>Jaffa Aharonov</v-toolbar-title>
    </v-toolbar> -->
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
      clipped: false,
      drawer: true,
      fixed: false,
      // items: [{
      //   icon: 'bubble_chart',
      //   title: 'Inspire'
      // }],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Jaffa Aharonov'
    }
  },
  name: 'App'
}
</script>
