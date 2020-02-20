<template>
  <v-carousel :show-arrows="false" :height="760">
    <v-carousel-item
      v-for="(image,index) in images"
      :key="index"
      :src="image.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    >
      <div class="carousel-text">
        <p class="mb-0">{{image.text}}</p>
        <p class="subText" v-if="image.subtext != '' ">{{image.subtext}}</p>
        <p v-else class="mb-5"></p>
        <v-btn color="#9577c2" class="app-btn" x-large>{{image.btn_text}}</v-btn>
      </div>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  data() {
    return {
      images: [
        {
          src:
            "https://ld-wp.template-help.com/wordpress_60118/wp-content/uploads/2016/05/pic001.jpg",
          text: "Self-publishing ",
          subtext: "can be your pathway to success!",
          btn_text: "read More"
        },
        {
          src:
            "https://ld-wp.template-help.com/wordpress_60118/wp-content/uploads/2016/05/pic002.jpg",
          text: "Write your own success ",
          subtext: "",
          btn_text: "publish today"
        }
      ]
    };
  }
};
</script>
<style scoped>
.carousel-text {
  position: relative;
  top: 230px;
  left: 390px;
  width: 950px;
}
.carousel-text p {
  color: white;
  font-family: inherit;
  font-size: 100px;
  text-transform: uppercase;
  line-height: 1em;
  letter-spacing: 0.04em;
}
.carousel-text .subText {
  font-size: 38px;
  text-transform: lowercase;
  font-family: Josefin Sans, sans-serif !important;
  margin: 15px 0px !important;
  font-weight: 600;
  letter-spacing: 0.04em;
  line-height: 1.31;
}

</style>