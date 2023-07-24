<template>
  <div class="about section" id ="aboutpage">
    <div class="title is-size-1 has-text-left">About Me</div>
    <div class="main">
      <div class="columns is-centered">
        <div class="column is-8-mobile is-4-tablet is-3-desktop">
          <img src="../assets/pfpic.jpg" class="profile-image" />
        </div>
        <div class="column is-10-mobile is-8-tablet is-6-desktop">
          <div class="about-text has-text-left">
            <h5 class="is-size-3-mobile">Who am I?</h5>
            <p class="is-size-5-mobile is-size-4-tablet">
              Hi! My name is Laviele Trias. I am currently a third year BS
              Computer Science Student studying at the University of the
              Philippines Visayas.
              <br>
              <br>
              I currently live in Iloilo City, Philippines.
              <br>
              <br>
              I am also the founder and president of the first-ever premiere
              Esports Organization in the University of the Philippines Visayas,
              UPV Diwata Esports.
              <br>
              <br>
              I like to play video games in my spare time as well as read and
              write books.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
/* About Page */
@import "~bulma/css/bulma.css";

* {
  background-color: #141416;
}

.about {
  padding: 50px 0px; /* Adjusted padding for better spacing */
  background-color: #141416;
}

.title {
  margin-bottom: 20px;
  font-family: "Prompt", sans-serif;
  background: -webkit-linear-gradient(316deg, #af40ff, #00ddeb 30%, #5b42f3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: bold;
  margin-left:15rem;
}
.column{
  margin-left: 5rem;
}

.main {
  display: flex;
  align-items: center;
  justify-content: center;
}

.profile-image {
  max-width: 100%;
  border-radius: 10px;
  margin: 1rem;
}

.about-text h5 {
  color: #cc0000;
  letter-spacing: 2px;
  font-size: 40px;
  margin-bottom: 25px;
  margin-top: 20px;
  background: -webkit-linear-gradient(144deg, #4a00e0 30%, #8e2de2);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-family: "Bebas Neue", sans-serif;
}

.about-text p {
  color: white;
  letter-spacing: 1px;
  line-height: 30px; /* Adjusted line-height for better spacing */
  font-size: 18px; /* Adjusted font size for better readability */
  margin-bottom: 10px;
  font-family: "Palanquin", sans-serif;
}
</style>
