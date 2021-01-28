<template>
  <NavBar />
  <Banner />
  <Services />
</template>

<script>
import NavBar from "./components/ui/NavBar.vue";
import Banner from "./components/Banner.vue";
import Services from "./components/Services.vue";

export default {
  name: "App",
  components: {
    NavBar,
    Banner,
    Services,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Fira+Sans:wght@300;400;500;600;700;800;900&display=swap");

#app {
  font-family: "Fira sans", Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
