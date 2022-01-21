<template>
  <v-container class="pt-15 mt-12">
    <v-row>
      <v-col lg-6>
        <img  width="100%" height="470" src="./../assets/1.jpg" alt="">
      </v-col>
      <v-col lg-6>
        <v-subheader class="text--h4" style="font-size: 30px">About Us</v-subheader>
        <p class="ml-4">It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here, content here', making it look like readable English. Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text,</p>

        <v-list>
          <v-list-item>
            <v-icon color="success" class="mr-4">mdi-check-all</v-icon>
            <v-list-item-subtitle>It is a long established fact that a reader</v-list-item-subtitle>
          </v-list-item>
          <v-list-item>
            <v-icon color="success" class="mr-4">mdi-check-all</v-icon>
            <v-list-item-subtitle>It will be distracted by the readable content of a page</v-list-item-subtitle>
          </v-list-item>
          <v-list-item>
            <v-icon color="success" class="mr-4">mdi-check-all</v-icon>
            <v-list-item-subtitle>when looking at its layout. The point of using </v-list-item-subtitle>
          </v-list-item>
        </v-list>
        <p class="ml-4">It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.
          The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here, content here</p>

      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "AboutComponent"
}
</script>

<style scoped>

</style>