<template>
  <div>
    <v-row
      ><v-col cols="12"
        ><v-carousel hide-delimiters hide-delimiters-background height="85vh">
          <v-carousel-item
            v-for="banner in 5"
            :key="banner"
            src="https://wallpapercave.com/wp/wp1915248.jpg"
          ></v-carousel-item>
        </v-carousel>
      </v-col>
    </v-row>
    <v-container><Homecard class="mt-n16" /></v-container>
    <v-parallax
      src="https://i.imgur.com/EHAZMJi.jpeg"
      class="mt-16 d-flex align-center justify-center"
      height="500"
    >
      <v-container>
        <v-row class="d-flex align-center">
          <v-col cols="12" md="4"
            ><v-img
              src="https://whitelabel.2u.com/cdn/v1/5892510e-fbcf-4dd5-8121-bb9246e7b0d6/marketing/logo-1.png"
            ></v-img
            ><v-card-title class="text-h4 font-weight-bold">
              Сургуулийн тухай
            </v-card-title></v-col
          >
          <v-col cols="12" md="8" class="px-2 px-md-10"
            ><v-card-text style="color: white">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam
              sit amet mattis ligula. Aliquam sagittis, libero ac ullamcorper
              mollis, nibh erat fermentum dui, id eleifend arcu libero quis
              enim. Phasellus purus nisl, porttitor vitae iaculis bibendum,
              ornare sit amet sapien. Donec finibus nec massa pellentesque
              sodales. Praesent ipsum augue, varius et sapien eu, venenatis
              semper odio. Duis consectetur eget dui sit amet congue. Praesent
              volutpat, ex ac lobortis efficitur, orci ex mattis lacus, sed
              fermentum nisi sapien quis sapien. Nulla nec bibendum massa. Donec
              nec maximus lorem, at dictum odio. Nullam venenatis, dolor eu
              dictum blandit, lorem ex vestibulum est, non imperdiet nulla
              tortor eu lacus.
            </v-card-text>
            <v-card-text style="color: white">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam
              sit amet mattis ligula. Aliquam sagittis, libero ac ullamcorper
              mollis, nibh erat fermentum dui, id eleifend arcu libero quis
              enim. Phasellus purus nisl, porttitor vitae iaculis bibendum,
              ornare sit amet sapien. Donec finibus nec massa pellentesque
              sodales. Praesent ipsum augue, varius et sapien eu, venenatis
              semper odio. Duis consectetur eget dui sit amet congue. Praesent
              volutpat, ex ac lobortis efficitur, orci ex mattis lacus, sed
              fermentum nisi sapien quis sapien. Nulla nec bibendum massa. Donec
              nec maximus lorem, at dictum odio. Nullam venenatis, dolor eu
              dictum blandit, lorem ex vestibulum est, non imperdiet nulla
              tortor eu lacus.
            </v-card-text></v-col
          ></v-row
        >
      </v-container>
    </v-parallax>
    <v-sheet color="#16213E" dark
      ><v-container
        ><v-row class="my-16"
          ><v-col cols="12" md="3"
            ><v-btn icon x-large color="success"
              ><v-icon>mdi-book</v-icon></v-btn
            ><v-card-title class="font-weight-bold text-h5">
              Lorem ipsum </v-card-title
            ><v-card-text>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam
              sit amet mattis ligula. Aliquam sagittis, libero ac ullamcorper
              mollis, nibh erat fermentum dui
            </v-card-text>
            <v-card-actions>
              <v-btn color="success" text small
                >цааш унших <v-icon small>mdi-arrow-right-thin</v-icon></v-btn
              >
            </v-card-actions></v-col
          >
          <v-col cols="12" md="3"
            ><v-btn icon x-large color="success"
              ><v-icon>mdi-earth</v-icon></v-btn
            ><v-card-title class="font-weight-bold text-h5">
              Lorem ipsum </v-card-title
            ><v-card-text>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam
              sit amet mattis ligula. Aliquam sagittis, libero ac ullamcorper
              mollis, nibh erat fermentum dui </v-card-text
            ><v-btn color="success" text small
              >цааш унших <v-icon small>mdi-arrow-right-thin</v-icon></v-btn
            ></v-col
          >
          <v-col cols="12" md="3"
            ><v-btn icon x-large color="success"
              ><v-icon>mdi-castle</v-icon></v-btn
            ><v-card-title class="font-weight-bold text-h5">
              Lorem ipsum </v-card-title
            ><v-card-text>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam
              sit amet mattis ligula. Aliquam sagittis, libero ac ullamcorper
              mollis, nibh erat fermentum dui </v-card-text
            ><v-btn color="success" text small
              >цааш унших <v-icon small>mdi-arrow-right-thin</v-icon></v-btn
            ></v-col
          >
          <v-col cols="12" md="3"
            ><v-btn icon x-large color="success"
              ><v-icon>mdi-certificate </v-icon></v-btn
            ><v-card-title class="font-weight-bold text-h5">
              Lorem ipsum </v-card-title
            ><v-card-text>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam
              sit amet mattis ligula. Aliquam sagittis, libero ac ullamcorper
              mollis, nibh erat fermentum dui </v-card-text
            ><v-btn color="success" text small
              >цааш унших <v-icon small>mdi-arrow-right-thin</v-icon></v-btn
            ></v-col
          >
        </v-row>
      </v-container></v-sheet
    >
    <Homenews class="mt-16 d-none d-md-flex" />
    <v-container grid-list-xs class="d-flex justify-center">
      <v-card-title primary-title> News </v-card-title>
    </v-container>

    <v-container grid-list-xs> <Newscard /> </v-container>
  </div>
</template>

<script>
import Homecard from "../components/homecard.vue";
import Homenews from "../components/homenews.vue";
import Newscard from "../components/newscard.vue";
export default {
  name: "IndexPage",
  components: { Homecard, Homenews, Newscard },
};
</script>
