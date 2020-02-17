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

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Lato');
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
</style>
