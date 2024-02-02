<template>
<nav class = "navbar">
  <div class="navbar-brand">
    <a class="navbar-item">
      <img src="https://i.imgur.com/H3lKnVi.png" width="30" height="40">
    </a>
    <div class="navbar-burger" data-target="navbarlist">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </div>


  <div id="navbarlist" class="navbar-menu">
    <div class="navbar-start">
      <div class="navbar-item">
        <div class="button is-black">Laviele Trias</div>
      </div>
    </div>
    <div class="navbar-end">
      <div class="navbar-item">
        <div class="field is-grouped">
          <p class="control">
            <a class="button is-black" href="#aboutpage">
              <span>About Me</span>
            </a>
          </p>
          <p class="control">
            <a class="button is-black" href="#education">
              <span>Education</span>
            </a>
          </p>
          <p class="control">
            <a class="button is-black" href="#skills">
              <span>Skills</span>
            </a>
          </p>
          <p class="control">
            <a class="button is-black" href="#contact">
              <span>Contact Me</span>
            </a>
          </p>
        </div>
      </div>
    </div>
  </div>
</nav>

  <section class="hero is-medium herobg">
    <div class ="hero-body">
      <div class ="container">
        <h1 class="title is-1 herocontent">Hello, world!</h1>
        <h2 class="subtitle herocontent">My name is Laviele Trias. I am an aspiring software developer.</h2>
      </div>
    </div>
  </section>
  </template>

<style lang="scss" scoped>
@import "~bulma/css/bulma.css";

.navbar-menu {
  background-color: #141416;
}
.navbar {
  font-family: "Prompt", sans-serif;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #141416;
  color: white;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  width: 100%;
  z-index: 999;
}

/* Landing Page */

.herobg{
  background-image: url('../assets/homebg.jpg'); /* Replace with your image path */
      background-size: cover;
      background-position: center center;
      height: 400px; /* Set a height for the hero section */
      color: white; /* Adjust text color for better visibility */
}

.herocontent{
  color:white;
  font-family: "Prompt", sans-serif;
}
</style>