<template>
  <div class="about section" id="education">
    <div class="title is-size-1 has-text-left">Education</div>
    <div class="main">
      <div class="box has-text-left">
        <div class="about-text">
          <h2 class="is-size-3-mobile is-size-2-tablet has-text-left">
            University of the Philippines Highschool in Iloilo
          </h2>
          <h5 class="is-size-4-mobile is-size-3-tablet has-text-left">
            High School and Senior High School - Humanities and Social Sciences
          </h5>
          <p class="is-size-5-mobile is-size-6-tablet has-text-left">
            Research: Mga Banas ng Kabisayaan: The Interest Level Towards
            Visayan Folklore Among Elementary Students
          </p>
          <p class="is-size-5-mobile is-size-6-tablet has-text-left">
            Elected as HUMSS Batch Business Manager in 2019
          </p>
          <p class="is-size-5-mobile is-size-6-tablet has-text-left">
            Elected as Business Manager for the UPHSI Computer Club in 2019
          </p>
          <p class="is-size-5-mobile is-size-6-tablet has-text-left">
            Elected as HUMSS Batch Vice President in 2019
          </p>
          <p class="is-size-5-mobile is-size-6-tablet has-text-left">
            Awarded by Junior Chamber International - Philippine Youth
            Leadership Excellence Award in 2014
          </p>
        </div>
        <div class="about-text">
          <h2 class="is-size-3-mobile is-size-2-tablet">
            University of the Philippines Visayas
          </h2>
          <h5 class="is-size-4-mobile is-size-3-tablet">
            College - Bachelor of Science in Computer Science
          </h5>
          <p class="is-size-5-mobile is-size-6-tablet">
            Relevant Coursework: Software Engineering, Mobile Development,
            Database Systems, Machine Level Programming
          </p>
          <p class="is-size-5-mobile is-size-6-tablet">
            Awarded as a Dean’s Lister / College Scholar in 2022
          </p>
          <p class="is-size-5-mobile is-size-6-tablet">
            Founded and became the President of UPV Diwata Esports in 2022
          </p>
          <p class="is-size-5-mobile is-size-6-tablet">
            Member of Google Developer Student Club
          </p>
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
  padding: 50px 0px; 
  background-color: #141416;
}

.title {
  margin-bottom: 20px;
  font-family: "Prompt", sans-serif;
  background: -webkit-linear-gradient(316deg, #af40ff, #00ddeb 30%, #5b42f3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: bold;
  margin-left: 15rem;
}

.main {
  display: flex;
  align-items: left;
  justify-content: left;
}

.about-text h2 {
  font-size: 40px;
  margin-bottom: 20px;
  font-family: "Prompt", sans-serif;
  background: -webkit-linear-gradient(144deg, #af40ff, #00ddeb 50%, #5b42f3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin-left: 15rem;
}

.about-text h5 {
  color: #cc0000;
  letter-spacing: 2px;
  font-size: 28px; 
  margin-bottom: 20px;
  background: -webkit-linear-gradient(144deg, #4a00e0 30%, #8e2de2);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-family: "Bebas Neue", sans-serif;
  margin-left: 15rem;
}

.about-text p {
  color: white;
  letter-spacing: 1px;
  line-height: 30px; 
  font-size: 18px; 
  margin-bottom: 10px;
  font-family: "Palanquin", sans-serif;
  margin-left: 15rem;
}

/* Responsive Typography */
@media screen and (max-width: 768px) {
  .about-text h2 {
    font-size: 30px;
    margin-left: 0;
  }
  .about-text h5 {
    font-size: 24px;
    margin-left: 0;
  }
  .about-text p {
    font-size: 16px;
    margin-left: 0;
  }
}
</style>
