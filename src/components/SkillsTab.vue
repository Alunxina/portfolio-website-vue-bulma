<template>
  <div class="skills" id="skills">
    <div class="title is-size-1 has-text-left">Programming Languages</div>
    <div class="cardmain columns is-multiline">
      <!-- Added is-multiline class -->
      <div class="column is-12-mobile is-6-tablet is-6-desktop">
        <!-- Adjusted column sizes for different screen sizes -->
        <div class="card">
          <div class="card-content">
            <h1>Python</h1>
            <progress
              id="progressbar"
              value="70"
              max="100"
              style="height: 24px; width: 40%"
            ></progress>
          </div>
        </div>
      </div>

      <div class="column is-12-mobile is-6-tablet is-6-desktop">
        <!-- Repeat this div for other cards -->
        <div class="card">
          <div class="card-content">
            <h1>C</h1>
            <progress
              id="progressbar"
              value="80"
              max="100"
              style="height: 24px; width: 40%"
            ></progress>
          </div>
        </div>
      </div>

      <div class="column is-12-mobile is-6-tablet is-6-desktop">
        <!-- Adjusted column sizes for different screen sizes -->
        <div class="card">
          <div class="card-content">
            <h1>JavaScript</h1>
            <progress
              id="progressbar"
              value="50"
              max="100"
              style="height: 24px; width: 40%"
            ></progress>
          </div>
        </div>
      </div>

      <div class="column is-12-mobile is-6-tablet is-6-desktop">
        <!-- Adjusted column sizes for different screen sizes -->
        <div class="card">
          <div class="card-content">
            <h1>Assembly</h1>
            <progress
              id="progressbar"
              value="80"
              max="100"
              style="height: 24px; width: 40%"
            ></progress>
          </div>
        </div>
      </div>

      <div class="column is-12-mobile is-6-tablet is-6-desktop">
        <!-- Adjusted column sizes for different screen sizes -->
        <div class="card">
          <div class="card-content">
            <h1>Flutter</h1>
            <progress
              id="progressbar"
              value="60"
              max="100"
              style="height: 24px; width: 40%"
            ></progress>
          </div>
        </div>
      </div>

      <div class="column is-12-mobile is-6-tablet is-6-desktop">
        <!-- Adjusted column sizes for different screen sizes -->
        <div class="card">
          <div class="card-content">
            <h1>PHP</h1>
            <progress
              id="progressbar"
              value="70"
              max="100"
              style="height: 24px; width: 40%"
            ></progress>
          </div>
        </div>
      </div>

      <div class="column is-12-mobile is-6-tablet is-6-desktop">
        <!-- Adjusted column sizes for different screen sizes -->
        <div class="card">
          <div class="card-content">
            <h1>Java</h1>
            <progress
              id="progressbar"
              value="50"
              max="100"
              style="height: 24px; width: 40%"
            ></progress>
          </div>
        </div>
      </div>

      <div class="column is-12-mobile is-6-tablet is-6-desktop">
        <!-- Adjusted column sizes for different screen sizes -->
        <div class="card">
          <div class="card-content">
            <h1>MySQL</h1>
            <progress
              id="progressbar"
              value="60"
              max="100"
              style="height: 24px; width: 40%"
            ></progress>
          </div>
        </div>
      </div>

      <div class="column is-12-mobile is-6-tablet is-6-desktop">
        <!-- Adjusted column sizes for different screen sizes -->
        <div class="card">
          <div class="card-content">
            <h1>Version Control</h1>
            <progress
              id="progressbar"
              value="70"
              max="100"
              style="height: 24px; width: 40%"
            ></progress>
          </div>
        </div>
      </div>

      <!-- Add other cards for different programming languages here -->
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "~bulma/css/bulma.css";

/* About Page */

/* Skills Card display */
.title {
  margin-bottom: 20px;
  font-family: "Prompt", sans-serif;
  background: -webkit-linear-gradient(316deg, #af40ff, #00ddeb 30%, #5b42f3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: bold;
  margin-left: 15rem;
}
.cardmain {
  margin-top: 100px;
  margin-left: 10rem;
  margin-right: 10rem;
}

.card {
  width: 100%;
  position: relative;
  border-radius: 20px;
  padding: 5px;
  transition: all 0.5s;
  background-image: linear-gradient(144deg, #af40ff, #5b42f3 50%, #00ddeb);
}

.card-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: rgb(5, 6, 45);
  border-radius: 10px;
  width: 100%;
  height: auto;
  height: 100px;
}

.card-content h1 {
  color: white;
  font-size: 25px;
  text-align: left;
  padding-left: 5rem;
  margin: 0;
  font-family: "Prompt", sans-serif;
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
