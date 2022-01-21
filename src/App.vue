<template>
  <v-app>
    <Header/>
    <HeroSection/>
    <About/>
    <Portfolio/>
    <Project/>
    <Gallery/>
    <Contact/>
    <Footer/>

    <v-main>

    </v-main>
  </v-app>
</template>

<script>

import Header from "./components/Header";
import HeroSection from "./components/HeroComonent"
import About from "./components/AboutComponent"
import Portfolio from "./components/PortfolioComponent"
import Project from "./components/ProjectComponent"
import Gallery from "./components/GalleryComponent"
import Contact from "./components/ContactUsComponent"
import Footer from "./components/FooterComponent"
export default {
  components: {
     Header,
    HeroSection,
    About,
    Portfolio,
    Project,
    Gallery,
    Contact,
    Footer
  },
  data(){
    return{

    }
  }
};
</script>
