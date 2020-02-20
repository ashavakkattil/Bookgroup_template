<template>
  <v-row class="subscribeMail">
    <v-col>
      <v-text-field placeholder="Your Email" outlined dark></v-text-field>
      <v-btn x-large class="app-btn subscribe-btn" dark>Subscribe</v-btn>
    </v-col>
  </v-row>
</template>

<style scoped>
.subscribeMail {
  align-items: baseline;
  width: 30%;
  margin: 0 auto;
}
.subscribe-btn {
  position: relative;
  left: 315px;
  bottom: 109px;
  height: 55px !important;
  border-radius: 0px 4px 4px 0px;
}
</style>