<template>
  <section>
    <div class="container">
      <div class="content has-text-left">
        <br><br>
        <h1 class="title">{{ pageTitle }}</h1>
        <div class="columns">
          <div class="column is-one-quarter">
            <img src="../assets/pfpic.jpg" class="profile-image" />
          </div>
          <div class="column">
            <h2 class="subtitle my-4">{{ subtitle }}</h2>
            <p class="my-4">{{ intro }}</p>
            <p class="my-4">{{ experience }}</p>
            <p>{{ hobbies }}</p>
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
      pageTitle: 'About Me',
      subtitle: 'Who am I?',
      intro: 'Hi! My name is Laviele Trias. I am currently a fourth-year BS Computer Science Student studying at the University of the Philippines Visayas.',
      experience: 'I have interned as a frontend web developer at DTE Endurance Asia. I have interests in machine learning and data science and have joined the UP Data Science Society to train my data science skills and gain experience. I am also the founder and president of the first-ever premiere Esports Organization in the University of the Philippines Visayas, UPV Diwata Esports.',
      hobbies: 'I like to play video games and read books in my spare time.',
    };
  },
};
</script>

<style lang="scss" scoped>
/* About Page */
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
  font-size:3rem;
}
h2 {
  font-size: 2rem;
  margin-bottom: 2rem;
  margin-top: 2rem;
  background: -webkit-linear-gradient(144deg, #4a00e0 30%, #8e2de2);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-family: "Prompt", sans-serif;
  font-weight:bold;
}

p {
  color: white;
  letter-spacing: 1px;
  line-height: 30px; 
  font-size: 18px; 
  margin-bottom: 10px;
  font-family: "Palanquin", sans-serif;
}
.profile-image {
  max-width: 100%;
  border-radius: 10px;
}


</style>