<template>
  <v-container>
    <v-row class="text-center">
      <v-col sm="12" md="4" v-for="(item,i) in book_items" :key="i" class="pb-10">
        <v-card class="bookgridCard" flat>
          <v-img :src="item.src"></v-img>
          <v-card-title class="gridCardTitle" v-if="$vuetify.breakpoint.lgAndUp">
            <h2>{{item.title}}</h2>
          </v-card-title>
          <v-card-title class="gridCardTitle gridCardTitleMdAndDown" v-else>
            <h2>{{item.title}}</h2>
          </v-card-title>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
export default {
  data() {
    return {
      book_items: [
        {
          title: "Self-publishing",
          src:
            "https://ld-wp.template-help.com/wordpress_60118/wp-content/uploads/2016/05/pic004.jpg"
        },
        {
          title: "Book Design",
          src:
            "https://ld-wp.template-help.com/wordpress_60118/wp-content/uploads/2016/05/pic005.jpg"
        },
        {
          title: "Book Marketing",
          src:
            "https://ld-wp.template-help.com/wordpress_60118/wp-content/uploads/2016/05/pic006.jpg"
        },
        {
          title: "Editorial Services",
          src:
            "https://ld-wp.template-help.com/wordpress_60118/wp-content/uploads/2016/05/pic007.jpg"
        },
        {
          title: "Solicitation & Publishing",
          src:
            "https://ld-wp.template-help.com/wordpress_60118/wp-content/uploads/2016/05/pic008.jpg"
        },
        {
          title: "E-Book Promotion",
          src:
            "https://ld-wp.template-help.com/wordpress_60118/wp-content/uploads/2016/05/pic009.jpg"
        }
      ]
    };
  }
};
</script>

<style scoped>

.bookGridCard {
  background-color: white;
}
.gridCardTitle {
  padding: 38px 25px 30px;
  justify-content: center;
}
.gridCardTitle h2 {
  font-family: Josefin Sans;
  letter-spacing: 0.04em;
  font-weight: 600;
}
.gridCardTitleMdAndDown h2 {
  font-size: 22px;
}
</style>