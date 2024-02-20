
<template>
  <section class="hero is-fullwidth" id="skills">
    <div class="hero-body">
      <div class="container has-text-left">
        <h1 class="title">Programming Languages and Skills</h1>
      </div>
    </div>

    <div class="hero-foot is-fullwidth">
      <nav class="tabs is-boxed is-fullwidth is-large">
        <div class="container">
          <ul>
            <li v-for="(tab, index) in tabs" :key="index" class="tab" @click="openTab(index)">
              <a>{{ tab.label }}</a>
            </li>
          </ul>
        </div>
      </nav>
    </div>

    <div class="container section is-fullwidth">
      <div v-for="(tab, index) in tabs" :key="index" :id="tab.id" class="content-tab" :style="{ display: currentTabIndex === index ? 'block' : 'none' }">
        <div class="columns">
          <div v-for="(item, itemIndex) in tab.items" :key="itemIndex" class="column">
            <img :src="item.image" :width="item.width" :height="item.height" />
            <p>{{ item.name }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      currentTabIndex: 0,
      tabs: [
        {
          id: 'languages',
          label: 'Languages',
          items: [
          { name: 'Python', image: require('../assets/python.png'), width: 40, height: 60 },
            { name: 'C', image: require('../assets/c.png'), width: 40, height: 60 },
            { name: 'JavaScript', image: require('../assets/javascript.png'), width: 40, height: 60 },
            { name: 'NASM', image: require('../assets/assembly.svg'), width: 40, height: 60 },
            { name: 'HTML', image: require('../assets/html.png'), width: 40, height: 60 },
            { name: 'CSS', image: require('../assets/css.png'), width: 40, height: 60 },
            { name: 'Flutter', image: require('../assets/flutter.png'), width: 40, height: 60 },
            { name: 'PHP', image: require('../assets/php.png'), width: 40, height: 60 },
            { name: 'Java', image: require('../assets/java.png'), width: 40, height: 60 },
          ],
        },
        {
          id: 'fworksdb',
          label: 'Frameworks and Database',
          items: [
            { name: 'Vue.js', image: require('../assets/vue.png'), width: 40, height: 60 },
            { name: 'GitHub', image: require('../assets/github.png'), width: 40, height: 60 },
            { name: 'Git', image: require('../assets/git.png'), width: 40, height: 60 },
            { name: 'MySQL', image: require('../assets/mysql.png'), width: 40, height: 60 },
          ],
        },
        {
          id: 'software',
          label: 'Software',
          items: [
            { name: 'Microsoft Office', image: require('@/assets/office.png'), width: 40, height: 60 },
            { name: 'Google Suite', image: require('../assets/gsuite.png'), width: 40, height: 60 },
            { name: 'Notion', image: require('../assets/notion.png'), width: 40, height: 60 },
            { name: 'Figma', image: require('../assets/figma.png'), width: 40, height: 60 },
            { name: 'Draw.io', image: require('../assets/draw-io.png'), width: 40, height: 60 },
          ],
        },
      ],
    };
  },
  methods: {
    openTab(index) {
      this.currentTabIndex = index;
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
