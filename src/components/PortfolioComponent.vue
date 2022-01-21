<template>
<v-container class="pt-15 mt-12">
  <v-row justify="center">
    <v-col lg='12' class="text-center">
      <v-subheader class="text-h4 justify-center" >Portfolio</v-subheader>
      <p>Lorem Ipsum is simply dummy text of the printing and typesetting</p>
    </v-col>
    <v-col lg="12">
      <div class="text-center">
        <v-chip @click="activePortfolio = 'webApp'" :color="activePortfolio == 'webApp' ? 'success' : ''" class="mx-5">Web App</v-chip>
        <v-chip @click="activePortfolio = 'mobileApp'" :color="activePortfolio=='mobileApp' ? 'success' : ''" class="mx-5">Mobile App</v-chip>
        <v-chip @click="activePortfolio = 'desktopApp'" :color="activePortfolio=='desktopApp' ? 'success' : ''" class="mx-5"> Desktop App</v-chip>
      </div>
    </v-col>
  <slot v-if="activePortfolio == 'webApp'">
    <v-col lg="3" v-for="(web,webindex) in webApp" :key="webindex">
      <v-card
          class="mx-auto"
          max-width="344"
      >
        <v-img
            src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
            height="200px"
        ></v-img>

        <v-card-title>
          {{web.title}}
        </v-card-title>
      </v-card>
    </v-col>
  </slot>
    <slot v-if="activePortfolio == 'mobileApp'">
      <v-col lg="3" v-for="(mobile,mobileindex) in mobileApp" :key="mobileindex">
        <v-card
            class="mx-auto"
            max-width="344"
        >
          <v-img
              src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
              height="200px"
          ></v-img>

          <v-card-title>
            {{mobile.title}}
          </v-card-title>
        </v-card>
      </v-col>
    </slot>
    <slot v-if="activePortfolio == 'desktopApp'">
      <v-col lg="3" v-for="(desktop,desktopindex) in desktopApp" :key="desktopindex">
        <v-card
            class="mx-auto"
            max-width="344"
        >
          <v-img
              :src="desktop.image"
              height="200px"
          ></v-img>

          <v-card-title>
            {{desktop.title}}
          </v-card-title>
        </v-card>
      </v-col>
    </slot>
  </v-row>
</v-container>
</template>

<script>
export default {
  name: "PortfolioComponent",
  data(){
    return{
      activePortfolio:'webApp',
      webApp:[
        {title:'Web App 1',image:''},
        {title:'Web App 2',image:''},
        {title:'Web App 3',image:''},
        {title:'Web App 4',image:''},
        {title:'Web App 5',image:''},
        {title:'Web App 6',image:''},
      ],
      mobileApp:[
        {title:'mobile App 1', image:''},
        {title:'mobile App 2', image:''},
        {title:'mobile App 2', image:''},
        {title:'mobile App 2', image:''},
        {title:'mobile App 2', image:''},
        {title:'mobile App2', image:''},
      ],
      desktopApp:[
        {title:'DesktopApp 1',image:'https://cdn.pixabay.com/photo/2020/07/12/07/47/bee-5396362_1280.jpg'},
        {title:'DesktopApp 2',image:'https://cdn.pixabay.com/photo/2020/07/12/07/47/bee-5396362_1280.jpg'},
        {title:'DesktopApp 3',image:'https://cdn.pixabay.com/photo/2020/07/12/07/47/bee-5396362_1280.jpg'},
        {title:'DesktopApp 4',image:'https://cdn.pixabay.com/photo/2020/07/12/07/47/bee-5396362_1280.jpg'},
        {title:'DesktopApp 5',image:'https://cdn.pixabay.com/photo/2020/07/12/07/47/bee-5396362_1280.jpg'},
        {title:'DesktopApp 6',image:'https://cdn.pixabay.com/photo/2020/07/12/07/47/bee-5396362_1280.jpg'},
      ]
    }
  }
}
</script>

<style scoped>

</style>