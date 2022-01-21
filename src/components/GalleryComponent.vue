<template>
<v-container  class="pt-15 mt-12">
  <v-row justify="center">
    <v-col lg="12" class="text-center">
      <v-subheader class="text-h4 justify-center">Our Gallery</v-subheader>
      <p>Lorem Ipsum is simply dummy text of the printing and typesetting</p>
    </v-col>
  </v-row>
  <v-row>
    <v-col lg="3"
        v-for="n in 12"
        :key="n"
        class="d-flex child-flex"
        cols="4"
    >
      <v-img
          :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
          :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
          aspect-ratio="1"
          class="grey lighten-2"
      >
        <template v-slot:placeholder>
          <v-row
              class="fill-height ma-0"
              align="center"
              justify="center"
          >
            <v-progress-circular
                indeterminate
                color="grey lighten-5"
            ></v-progress-circular>
          </v-row>
        </template>
      </v-img>
    </v-col>
  </v-row>
</v-container>
</template>

<script>
export default {
  name: "GalleryComponent"
}
</script>

<style scoped>

</style>