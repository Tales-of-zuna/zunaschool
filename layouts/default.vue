<template>
  <v-app dark style="background-color: #f3f7fb">
    <v-app-bar
      clipped-left
      fixed
      app
      hide-on-scroll
      style="background-color: #16213e"
      dark
    >
      <v-btn plain class="ml-16" small
        ><v-icon class="mx-2">mdi-email</v-icon>contact@uzblas.edu</v-btn
      >
      <v-btn plain small><v-icon class="mx-2">mdi-phone</v-icon>89007861</v-btn>
      <v-spacer></v-spacer>
      <v-btn plain small>about us</v-btn>
      <v-btn plain small>something</v-btn>
      <v-btn plain small>холбоо барих </v-btn>
      <v-btn color="success" tile class="mr-16">бүртгүүлэх</v-btn>

      <template v-slot:extension>
        <!-- <v-app-bar-nav-icon color="#16213E" @click.stop="drawer = !drawer" /> -->
        <v-btn to="/" text class="ml-16"
          ><v-img
            width="150"
            src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/Harvard_University_logo.svg/2560px-Harvard_University_logo.svg.png"
          ></v-img
        ></v-btn>
        <v-spacer></v-spacer>
        <v-tabs class="d-none d-lg-flex justify-end" light color="#16213E">
          <v-tab
            v-for="link in links"
            :key="link"
            :to="link.to"
            class="text-caption"
          >
            {{ link.title }}
          </v-tab>
        </v-tabs>
        <div class="mr-16"></div>
      </template>
    </v-app-bar>
    <v-main>
      <Nuxt />
    </v-main>

    <v-footer>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {
      products: [],
      tabs: [
        {
          title: "Сургалт",
          to: "/",
          icon: "book-education",
        },
      ],
      links: [
        {
          title: "нүүр",
          to: "/",
        },
        {
          title: "сургалт ",
          to: "/education",
        },
        {
          title: "Бидний амжилт",
          to: "/achievement",
        },
        {
          title: "Сургуулийн тухай",
          to: "/about",
        },
        {
          title: "Эцэг эхийн зөвлөл",
          to: "/parents",
        },
        {
          title: "мэдээ, мэдээлэл",
          to: "/parents",
        },
        {
          title: "Элсэлт",
          to: "/apply",
        },
      ],
    };
  },
};
</script>
<style>
div.v-toolbar__extension {
  background-color: white;
}
</style>
