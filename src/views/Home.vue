<template>
  <div class="home mt-8">
    <Slider />
    <v-container>
      <div class="info_container">
        <v-img src="../assets/info_icon.png"></v-img>
        <div class="info_message">
          <h5>Do you feel like the next Charles Dickens or Erik Larson?</h5>
          <p>
            Regardless of your writing being a fiction or a documentary work, we have a lot to offer,
            so you can bring your manuscript to the public eye!
          </p>
        </div>
      </div>
    </v-container>
  </div>
</template>

<script>
import Slider from "../components/Slider";
export default {
  name: "Home",
  components: { Slider }
};
</script>

<style scoped>
.info_container {
  text-align: center;
  padding-top: 66px;
  padding-bottom: 106px;
}
.info_container .v-image {
  height: 44px;
  widows: 44px;
  display: inline-flex;
}
.info_message {
  margin-top: 27px;
}
.info_message h5 {
  font-family: "Josefin Sans";
  font-size: 35px;
  letter-spacing: 0.04em;
  font-weight: 600;
  margin-bottom: 15px;
}
.info_message p{
  font-family: Lato, sans-serif;
  font-size: 17px;
  font-weight: 300;
  width: 40%;
  margin: 0 auto;
}
</style>
