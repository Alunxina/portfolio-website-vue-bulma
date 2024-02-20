<template>
  <div class="section" id="projects">
    <div class="container has-text-left">
      <h1 class="title">Projects</h1><br>
    </div>
    <div class="columns">
      <div class="column" v-for="project in projects" :key="project.id">
        <div class="card" @click="redirect(project.link)">
          <div class="card-content">
            <img :src="project.image" :width="project.width" :height="project.height">
            <div class="has-text-left">
              <p class="my-3">{{ project.title }}</p>
              <p>
                <small>{{ project.role }}</small><br>
                {{ project.description }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<!-- Your existing script and style sections remain unchanged -->


<script>
export default {
  data() {
    return {
      projects: [
        {
          id: 1,
          title: "Lagaw: Iloilo City's Travel App",
          role: "Project Manager, Front-end Web Developer, UI/UX",
          description:
            "Lagaw is a web application made for travellers who want to visit Iloilo City...",
          link: "https://github.com/Cmpdleon/cmsc129",
          image: require("../assets/lagaw.png"),
          width: 500,
          height: 500
        },
        {
          id: 2,
          title: "Address Locator Using Vue",
          role: "Front-end Developer",
          description:
            "Address locator using vue, bulma, vue router, and vuex.",
          link:
            "https://github.com/vieletrias/vue-address-locator",
          image: require("../assets/addresslocator.png"),
          width: 500,
          height: 500
        },
        {
          id: 3,
          title: "Esports Website",
          role: "Fullstack Web Developer",
          description:
            "Simple website implementing HTML, CSS and Javascript",
          link: "https://github.com/vieletrias/vue-address-locator",
          image: require("../assets/diwatawebsite.png"),
          width: 500,
          height: 500
        },
        // Add other projects here
      ],
    };
  },
  methods: {
    redirect(link) {
      window.location.href = link;
    },
  },
};
</script>


<style lang="scss" scoped>
@import "~bulma/css/bulma.css";

.section {
  background-color: #141416;
}
.title {
  font-family: "Prompt", sans-serif;
  background: -webkit-linear-gradient(316deg, #af40ff, #00ddeb 30%, #5b42f3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: bold;
  font-size: 3rem;
}
.column {
  display: flex;
  background-color: #141414;
}


.card {
  height:auto;
  width: auto;
  position: relative;
  border-radius: 20px;
  padding: 5px;
  transition: all 0.5s;
  background-image: linear-gradient(144deg, #af40ff, #5b42f3 50%, #00ddeb);
  cursor: pointer;
}
.card-content {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: flex-start;
  background: rgb(5, 6, 45);
  border-radius: 10px;
  padding: 1.5rem;
}

.card-content p {
  color: white;
  font-size: 1rem;
  margin-bottom: 1.5rem;
  font-family: "Prompt", sans-serif;
}
.card:hover {
  transform: scale(1.05);
  background: linear-gradient(315deg, #ff0058, #03a9f4);
}

body {
  background-color: #141416;
}

</style>
