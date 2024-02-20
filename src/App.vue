<template>
    <head>
    <link rel="icon" href="../assets/avatar.png">
    <title>Laviele Trias</title>
  </head>
  <NavBar />
  <AboutTab />
  <SkillsTab />
  <ProjectsTab />
  <ContactTab />
</template>

<script>
import NavBar from "./components/NavBar.vue";
import AboutTab from "./components/AboutTab.vue";
import SkillsTab from "./components/SkillsTab.vue";
import ProjectsTab from "./components/ProjectsTab.vue";
import ContactTab from "./components/ContactTab.vue";

export default {
  name: "App",
  components: {
    NavBar,
    AboutTab,
    SkillsTab,
    ProjectsTab,
    ContactTab,
  },
};
</script>

<style lang="scss">
@import "~bulma/css/bulma.css";

@import url('https://fonts.googleapis.com/css2?family=Prompt:wght@500&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Palanquin:wght@500&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Martel+Sans:wght@600&family=Palanquin:wght@500&display=swap');


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
html {
  scroll-behavior: smooth;
}
html,body{
    overflow-x: hidden;
}
</style>
