<template>
  <v-container grid-list-xs>
    <v-row
      ><v-col cols="6" md="3" v-for="medee in 6" :key="medee">
        <v-card to="/">
          <v-img
            src="https://news.mn/wp-content/uploads/2022/10/332BEDA6-702A-4033-AB3C-F6B3BCA0B0D1.jpeg"
          ></v-img>
          <v-card-title primary-title> news title 1 </v-card-title>
          <v-card-subtitle> 2022/10/21</v-card-subtitle>
          <v-card-text class="overflow-auto" height="150">
            Хятадын Коммунист намын Төв хорооны 370 орчим гишүүн хаалттай
            хаалганы цаана өнөөдөр (2022.10.9) Бээжинд хуралдаж байна.
          </v-card-text>
          <v-card-actions class="d-flex justify-center">
            <v-btn color="success" text>Цааш унших</v-btn>
          </v-card-actions>
        </v-card></v-col
      ></v-row
    >
  </v-container>
</template>

<script>
export default {};
</script>

<style></style>
