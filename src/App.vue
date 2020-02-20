<template>
  <v-app>
    <Appheader />
    <router-view></router-view>
  </v-app>
</template>

<script>
import Appheader from "./components/AppHeader";

export default {
  name: "App",

  components: {
    Appheader
  },

  data: () => ({
    //
  })
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Lato");
@import url("https://fonts.googleapis.com/css?family=Josefin+Sans");

#app {
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.625;
  font-family: Lato, sans-serif;
  letter-spacing: 0.04em;
  text-align: left;
  color: #323232;
}
.app-btn {
  margin: 23px 0px 0px;
  padding: 16px 66px !important;
  font-weight: 700;
  font-size: 13px;
  background-color: #9577c2 !important;
}
</style>
