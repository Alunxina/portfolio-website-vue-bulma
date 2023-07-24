<template>
  <div class="section" id="projects">
    <div class="title is-size-1 has-text-left">Projects and Contributions</div>
    <br /><br />
    <div class="columns">
      <div class="column">
        <div class="card" @click="LagawRedirect">
          <div class="box">
            <div class="block">
              <figure class="image is-5by3">
                <img src="../assets/lagaw.png" />
              </figure>
              <br />
              <div class="card-content">
                <div class="has-text-left">
                  <br />
                  <h1>Lagaw: Iloilo City's Travel App</h1>
                  <br />
                  <p>
                    <small
                      >Project Manager, Front-end Web Developer, UI
                      Designer</small
                    >
                    <br />
                    Lagaw is a web application made for travellers who want to
                    visit Iloilo City. It features a list of accomodations for
                    travellers who want to stay overnight as well as a list of
                    attractions that they can visit to along with several other
                    features.
                  </p>
                </div>
              </div>
              <button class="gradientbutton">
                <span>Access the Project</span>
              </button>
            </div>
          </div>
        </div>
      </div>

      <div class="column">
        <div class="card" @click="AroundUPVRedirect">
          <div class="box">
            <div class="block">
              <figure class="image is-5by3">
                <img src="../assets/aroundupv.png" />
              </figure>
              <br />
              <div class="card-content">
                <div class="has-text-left">
                  <br />
                  <h1>AroundUPV: A UPV Navigation App</h1>
                  <br />
                  <p>
                    <small>UI Designer</small>
                    <br />
                    AroundUPV is a proposed navigation application made for UPV
                    Students. It features a forum where students can ask the
                    community anything. It also features a list of restaurants,
                    boarding houses and several key locations, perfect for
                    freshmen who are just starting to get around the university.
                  </p>
                </div>
              </div>
              <button class="gradientbutton">
                <span>Access the Project</span>
              </button>
            </div>
          </div>
        </div>
      </div>

      <div class="column">
        <div class="card" @click="DiwataRedirect">
          <div class="box">
            <div class="block">
              <figure class="image is-5by3">
                <img src="../assets/diwatawebsite.png" />
              </figure>
              <br />
              <div class="card-content">
                <div class="has-text-left">
                  <br />
                  <h1>UPV Diwata Esports Website</h1>
                  <br />
                  <p>
                    <small>Fullstack developer, UI Designer</small>
                    <br />
                    This is a mockup of a website for the UPV Diwata Esports. It
                    features what Diwata Esports is all about as well as a
                    registration form should users want to join the
                    organization. Not only that, the UPV Diwata Esports Website
                    also features a gallery and the org's mission and vision.
                  </p>
                </div>
              </div>
              <button class="gradientbutton">
                <span>Access the Project</span>
              </button>
            </div>
          </div>
        </div>
      </div>

      <div class="column">
        <div class="card" @click="HobbitRedirect">
          <div class="box">
            <div class="block">
              <figure class="image is-5by3">
                <img src="../assets/hobbit.png" />
              </figure>
              <br />
              <div class="card-content">
                <div class="has-text-left">
                  <br />
                  <h1>Hobbit: Text Adventure</h1>
                  <br />
                  <p>
                    <small>UI Designer</small>
                    <br />
                    The hobbit text adventure is a Java based game that features
                    a short scenario about your life as a Hobbit living in the
                    Shire. Players can decide and choose the best decision in
                    certain scenarios and watch out for the other hobbits who
                    want to ruin your special event! Get the best ending and
                    help your uncle plan the perfect birthday!
                  </p>
                </div>
              </div>
              <button class="gradientbutton">
                <span>Access the Project</span>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    LagawRedirect() {
      window.location.href = "https://github.com/Cmpdleon/cmsc129";
    },

    AroundUPVRedirect() {
      window.location.href =
        "https://drive.google.com/file/d/1g-AY-J2_7v3YjFtYbj6PUi5sGU8FGcyI/view?usp=sharing";
    },

    DiwataRedirect() {
      window.location.href = "https://github.com/Alunxina/Trias-Website-Lab-1";
    },
    HobbitRedirect() {
      window.location.href =
        "https://github.com/Alunxina/Hobbit-Text-Adventure-Javadoc";
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
  margin-bottom: 20px;
  font-family: "Prompt", sans-serif;
  background: -webkit-linear-gradient(316deg, #af40ff, #00ddeb 30%, #5b42f3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: bold;
  margin-left: 11rem;
}
.column {
  display: flex;
  background-color: #141414;
}
.box {
  max-width: 400px;
  border-radius: 0.5rem;
  background-color: rgb(5, 6, 45);
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
  border: 1px solid transparent;
}

/* Projects and Contribution Cards */
.box a {
  text-decoration: none;
}

.content {
  padding: 1.1rem;
  cursor: pointer;
}

.box img {
  object-fit: cover;
  width: 100%;
  height: 250px;
  background-color: rgb(5, 6, 45);
  border-radius: 1px;
}

.title {
  color: white;
  font-size: 20px;
  line-height: 1.75rem;

  font-family: "Prompt", sans-serif;
}

.card {
  width: auto;
  height: auto;
  position: relative;
  border-radius: 20px;
  padding: 5px;
  transition: all 0.5s;
  background-image: linear-gradient(144deg, #af40ff, #5b42f3 50%, #00ddeb);
  cursor: pointer;
}

.card-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: rgb(5, 6, 45);
  border-radius: 10px;
  width: 100%;
  height: 26rem;
}

.card-content h1 {
  color: white;
  font-size: 1.5rem;
  text-align: left;
  margin: 0;
  font-family: "Prompt", sans-serif;
}
.card-content p {
  color: white;
}

.card-content progress {
  height: 24px;
  width: 80%;
  margin-right: 5rem;
}

.card:hover {
  transform: scale(1.05);
  background: linear-gradient(315deg, #ff0058, #03a9f4);
}

.skills {
  background-color: #141416;
}

.skillswrap {
  width: 100%;
  margin-left: 0;
  text-align: center; /* Center the h1 text on mobile */
}

.skillswrap h1 {
  margin-top: 5vh;
  font-size: 5rem;
  margin-bottom: 5vh; /* Add margin at the bottom for spacing */
  font-family: "Prompt", sans-serif;
}

.gradientbutton {
  position: relative;
  font-family: inherit;
  font-weight: 500;
  font-size: 18px;
  letter-spacing: 0.05em;
  border-radius: 0.8em;
  border: none;
  background: linear-gradient(to right, #8e2de2, #4a00e0);
  color: ghostwhite;
  overflow: hidden;
  width: 10rem;
  font-family: "Prompt", sans-serif;
  width: auto;
  cursor: pointer;
}

.gradientbutton a {
  text-decoration: none;
  color: white;
}

.gradientbutton span {
  position: relative;
  z-index: 10;
  transition: color 0.4s;
  display: inline-flex;
  align-items: center;
  padding: 0.8em 1.2em 0.8em 1.05em;
}

.gradientbutton::before,
.gradientbutton::after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 0;
}

.gradientbutton::before {
  content: "";
  background: #000;
  width: 120%;
  left: -10%;
  transform: skew(30deg);
  transition: transform 0.4s cubic-bezier(0.3, 1, 0.8, 1);
}

.gradientbutton:hover::before {
  transform: translate3d(100%, 0, 0);
}

.gradientbutton:active {
  transform: scale(0.95);
}

body {
  background-color: #141416;
}

/* Mobile responsive layout using Bulma classes */
@media screen and (max-width: 768px) {
  .cardmain {
    margin-left: 1rem;
    margin-right: 1rem;
  }
  .card-content h1 {
    padding-left: 1rem;
  }
}
</style>
