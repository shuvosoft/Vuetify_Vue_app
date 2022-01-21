<template>
  <v-container class="pt-15 mt-12" >
    <v-row>
      <v-col lg="6">
        <h2 class="banner-title">Welcome to our vuetify App</h2>
        <p class="banner-description">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s</p>
        <v-btn color="success" class="white--text mr-10" rounded>Get Started</v-btn>
        <v-btn color="indigo" class="white--text" rounded>
          <v-icon>mdi-play-circle</v-icon>Watch Video
        </v-btn>
      </v-col>
      <v-col lg="6">
        <img width="100%" src="./../assets/hero.png" alt="">

      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "HeroComonent"
}
</script>

<style scoped>
h2.banner-title{
  font-size: 60px;
  font-weight: bold;
  color: #444;
}
p.banner-description{
  font-size: 19px;
  margin: 32px 0px;
}
</style>