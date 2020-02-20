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
    <div class="menu-container" id="menu-container">
      <v-menu
        open-on-hover
        bottom
        offset-y
        content-class="app-menu"
        transition="slide-y-transition"
      >
        <template v-slot:activator="{ on }">
          <v-btn v-on="on" text class="menu-btn">Home</v-btn>
        </template>
        <v-list>
          <v-list-item>
            <v-list-item-title>header settings</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>Footer settings</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>Typography</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>Static Elements</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>FAQs</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>404</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>Documentation</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
      <v-menu content-class="app-menu">
        <template v-slot:activator="{ on }">
          <v-btn v-on="on" text class="menu-btn">About Us</v-btn>
        </template>
      </v-menu>
      <v-menu
        open-on-hover
        bottom
        offset-y
        content-class="app-menu"
        transition="slide-y-transition"
      >
        <template v-slot:activator="{ on }">
          <v-btn v-on="on" text class="menu-btn">Services</v-btn>
        </template>
        <v-list>
          <v-list-item>
            <v-list-item-title>Self-publishing</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>Editorial services</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>book design</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>solicitation & publishing</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
      <v-menu content-class="app-menu">
        <template v-slot:activator="{ on }">
          <v-btn v-on="on" text class="menu-btn">Pricing</v-btn>
        </template>
      </v-menu>
      <v-menu
        open-on-hover
        bottom
        offset-y
        content-class="app-menu"
        transition="slide-y-transition"
      >
        <template v-slot:activator="{ on }">
          <v-btn v-on="on" text class="menu-btn">Blog</v-btn>
        </template>
        <v-list>
          <v-list-item>
            <v-list-item-title>sidebar settings</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>post format</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>blog layout</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
      <v-menu content-class="app-menu">
        <template v-slot:activator="{ on }">
          <v-btn v-on="on" text class="menu-btn">Contact Us</v-btn>
        </template>
      </v-menu>
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
  padding: 43px 0px;
  width: 280px;
  margin: auto;
}
.menu-container {
  max-width: 900px;
  margin: 0px auto;
  text-align: center;
}
.app-menu {
  top: 270px !important;
  width: 200px !important;
  box-shadow: none !important;
  border: 1px solid #eee;
}
.menu-btn {
  padding: 0px 40px !important;
  text-transform: capitalize !important;
  font-family: Josefin Sans, sans-serif !important;
  font-size: 18px !important;
  font-weight: 700 !important;
  letter-spacing: 0.04em !important;
}
.menu-btn:hover {
  border-top: 3px solid #9577c2;
  border-radius: 0px;
  background: white;
  background-color: white;
  transition: 0.25s;
}
.app-menu .v-list-item {
  border-bottom: 1px solid #eee;
}
.app-menu .v-list-item__title {
  color: #9577c2;
  font-weight: 700;
  font-size: 1rem;
  text-transform: capitalize;
  font-family: Josefin Sans, sans-serif;
}
</style>