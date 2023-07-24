<template>
  <NavBar />
  <AboutTab />
  <EducationTab />
  <SkillsTab />
  <ProjectsTab />
  <ContactTab />
</template>

<script>
import NavBar from "./components/NavBar.vue";
import AboutTab from "./components/AboutTab.vue";
import EducationTab from "./components/EducationTab.vue";
import SkillsTab from "./components/SkillsTab.vue";
import ProjectsTab from "./components/ProjectsTab.vue";
import ContactTab from "./components/ContactTab.vue";

export default {
  name: "App",
  components: {
    NavBar,
    AboutTab,
    EducationTab,
    SkillsTab,
    ProjectsTab,
    ContactTab,
  },
};
</script>

<style lang="scss">
@import "~bulma/css/bulma.css";
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
</style>
