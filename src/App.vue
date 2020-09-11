<template>
  <div id="app">
    <Header />
    <HeroSction />
    <Process />
    <Services />
    <NewsLetter />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import HeroSction from "./components/HeroSection";
import Process from "./components/Process/Process";
import Services from "./components/Services/Services";
import NewsLetter from "./components/NewsLetter";
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    Header,
    HeroSction,
    Process,
    Services,
    NewsLetter,
    Footer
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Open Sans", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
