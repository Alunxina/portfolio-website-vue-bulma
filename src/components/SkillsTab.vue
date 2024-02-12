<template>
  <section class="hero is-fullwidth">
    <div class="hero-body">
      <div class="container has-text-left">
        <h1 class="title">Programming Languages and Skills</h1>
      </div>
    </div>

    <div class="hero-foot is-fullwidth">
      <nav class="tabs is-boxed is-fullwidth is-large">
        <div class="container">
          <ul>
            <ul>
              <li class="tab" @click="openTab('languages')">
                <a>Languages</a>
              </li>
              <li class="tab" @click="openTab('fworksdb')">
                <a>Frameworks and Database</a>
              </li>
              <li class="tab" @click="openTab('software')"><a>Software</a></li>
            </ul>
          </ul>
        </div>
      </nav>
    </div>

    <div class="container section is-fullwidth">
      <div id="languages" class="content-tab" ref="languages">
        <div class="columns">
          <div class="column">
            <img src="../assets/python.png" width="40" height="60" />
            <p>Python</p>
          </div>
          <div class="column">
            <img src="../assets/c.png" width="40" height="60" />
            <p>C</p>
          </div>
          <div class="column">
            <img src="../assets/javascript.png" width="40" height="60" />
            <p>Javascript</p>
          </div>
          <div class="column">
            <img src="../assets/assembly.svg" width="40" height="60" />
            <p>NASM</p>
          </div>
        </div>
        <div class="columns">
          <div class="column">
            <img src="../assets/html.png" width="40" height="60" />
            <p>HTML</p>
          </div>
          <div class="column">
            <img src="../assets/css.png" width="40" height="60" />
            <p>CSS</p>
          </div>
          <div class="column">
            <img src="../assets/flutter.png" width="40" height="60" />
            <p>Flutter</p>
          </div>
          <div class="column">
            <img src="../assets/php.png" width="40" height="60" />
            <p>PHP</p>
          </div>
          <div class="column">
            <img src="../assets/java.png" width="40" height="60" />
            <p>Java</p>
          </div>
        </div>
      </div>
      <div id="fworksdb" class="content-tab" style="display: none" ref="fworksdb">
        <div class="container section is-fullwidth">
          <div class="columns">
            <div class="column">
              <img src="../assets/vue.png" width="40" height="60" />
              <p>Vue.js</p>
            </div>
            <div class="column">
              <img src="../assets/github.png" width="40" height="60" />
              <p>Github</p>
            </div>
            <div class="column">
              <img src="../assets/git.png" width="40" height="60" />
              <p>Git</p>
            </div>
            <div class="column">
              <img src="../assets/mysql.png" width="40" height="60" />
              <p>MySQL</p>
            </div>
          </div>
        </div>
      </div>
      <div id="software" class="content-tab" style="display: none" ref="software">
        <div class="container section is-fullwidth">
          <div class="columns">
            <div class="column">
              <img src="../assets/vue.png" width="40" height="60" />
              <p>Microsoft Office</p>
            </div>
            <div class="column">
              <img src="../assets/mysql.png" width="40" height="60" />
              <p>Google Suite</p>
            </div>
            <div class="column">
              <img src="../assets/github.png" width="40" height="60" />
              <p>Notion</p>
            </div>
            <div class="column">
              <img src="../assets/git.png" width="40" height="60" />
              <p>Figma</p>
            </div>
            <div class="column">
              <img src="../assets/mysql.png" width="40" height="60" />
              <p>Draw.io</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    openTab(tabName) {
      this.$refs[tabName].style.display = "block";

      // Hide other tabs
      for (const refName in this.$refs) {
        if (refName !== tabName) {
          this.$refs[refName].style.display = "none";
        }
      }

      // Update tab classes
      const tablinks = document.querySelectorAll(".tab");
      tablinks.forEach((tab) => {
        tab.classList.remove("is-active");
      });
      event.currentTarget.classList.add("is-active");
    },
  },
};
</script>

<style lang="scss" scoped>
@import "~bulma/css/bulma.css";

* {
  background-color: #141416;
}

.title {
  margin-bottom: 2rem;
  font-family: "Prompt", sans-serif;
  background: -webkit-linear-gradient(316deg, #af40ff, #00ddeb 30%, #5b42f3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: bold;
  font-size: 3rem;
}

a {
  font-size: 2rem;
  margin-bottom: 2rem;
  margin-top: 2rem;
  background: -webkit-linear-gradient(144deg, #4a00e0 30%, #8e2de2);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-family: "Prompt", sans-serif;
  font-weight: bold;
}

p {
  color: white;
  letter-spacing: 1px;
  line-height: 30px;
  font-size: 18px;
  margin-bottom: 10px;
  font-family: "Palanquin", sans-serif;
}
</style>
