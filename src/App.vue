<template>
  <NavBar />
  <Banner />
  <Services />
  <Projects />
  <Contact />
</template>

<script>
import NavBar from "./components/ui/NavBar.vue";
import Banner from "./components/Banner.vue";
import Services from "./components/Services.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";

export default {
  name: "App",
  components: {
    NavBar,
    Banner,
    Services,
    Projects,
    Contact,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Fira+Sans:wght@300;400;500;600;700;800;900&display=swap");
#app {
  font-family: "Fira sans", Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin: -0.5em;
  padding: 0;
  box-sizing: border-box;
}
</style>
