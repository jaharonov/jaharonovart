<template>
  <v-container class="primary" fluid>
    <v-slide-y-transition mode="out-in">
      <v-layout column justify-space-around>
        <v-flex>
        <div class="landing-image-div">
        <img src="@/assets/pink_sheet_1.jpg" id="landing-selfie">
        </div>
        </v-flex>
        <br/>
        <v-flex>
        <div class="text">
        <h1 class="secondary">JAFFA AHARONOV</h1>
        <h3 class="accent">HI! I'M BEING REBUILT!</H3>
        </div>
        </v-flex>
      </v-layout>
    </v-slide-y-transition>
  </v-container>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
