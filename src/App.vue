<template>
  <div id="app">
    <Navbar />
    <Footer />
    <BannerSignUp />
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
import BannerSignUp from "./components/BannerSignUp.vue";
export default {
  name: "App",
  components: {
    Navbar,
    Footer,
    BannerSignUp,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
