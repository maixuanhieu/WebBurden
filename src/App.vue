<template>
  <v-app>
    <Header />

    <v-main>
      <!--Hero section-->

      <HeroComponent />

      <!--About us-->

      <Aboutus />

      <!--Portfolio-->

      <Portfolio />

      <!--Project-->
      <Project />

      <!--Gallery-->
      <Gallery />

        <!--Contact Us-->
        <Contactus />

        <!--Footer-->
        <Footer />
    </v-main>


  </v-app>
</template>

<script>
import Header from "./components/Header";
import HeroComponent from "./components/HeroComponent";
import Aboutus from "./components/Aboutus";
import Portfolio from "./components/Portfolio";
import Project from "./components/Project";
import Gallery from "./components/Gallery";
import Contactus from "./components/Contactus";
import Footer from "./components/Footer";
export default {
  name: "App",
  components: {Footer, Contactus, Gallery, Project, Portfolio, Aboutus, HeroComponent, Header},
  data() {
    return {
      menus: [
        { title: "Home", route: "home" },
        { title: "About us", route: "about-us" },
        { title: "Portfolio", route: "portfolio" },
        { title: "Project", route: "project" },
        { title: "Gallery", route: "gallery" },
        { title: "Contact", route: "contact" },
      ],
    };
  },
};
</script>
