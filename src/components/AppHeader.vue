<template>
  <div>
    <v-app-bar color="#f5f5f5" dense flat>
      <v-row class="top-panel ma-auto">
        <v-col class="social-group" sm="1">
          <v-icon size="20">mdi-facebook</v-icon>
          <v-icon class="ml-4" size="20">mdi-twitter</v-icon>
          <v-icon class="ml-4" size="20">mdi-google-plus</v-icon>
        </v-col>
        <v-col class="top-panel-message" sm="10">
          <v-row>
            <v-col sm="7">Powered by Experts. Published by you.</v-col>
            <v-col sm="2">
              Call Us Today
              <span class="font-weight-black">555.123.2323</span>
            </v-col>
            <v-col sm="3">22 St. Black Road Raleigh, PA 34578</v-col>
          </v-row>
        </v-col>
        <v-col class="search-bar" sm="1">
          <v-text-field
            class="search-text-bar"
            outlined
            dense
            single-line
            placeholder="Search..."
            append-icon="mdi-magnify"
          ></v-text-field>
        </v-col>
      </v-row>
    </v-app-bar>
    <div class="logo-container">
      <v-img src="../assets/logo.png" />
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      isClicked: false,
      showIcon: true
    };
  }
};
</script>
<style >
.top-panel {
  margin: 0 auto;
  max-width: 1730px;
  height: inherit;
}
.top-panel .col {
  height: inherit;
}
.search-text-bar .v-input__control .v-input__slot {
  min-height: 20px !important;
}
.top-panel-message {
  font-size: 14px;
}
.top-panel-message .col {
  padding: 0px;
}
.logo-container {
  padding: 54px 6rem 11px;
  width: 480px;
  margin: auto;
}
</style>