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
      <div class="navbar-item has-text-white">
          Laviele Trias
        </div>
    </div>
    <div class="navbar-end">
      <div class="navbar-item">
        <div class="field is-grouped">
          <p class="control">
            <a class="button is-black gradientbutton" href="#aboutpage">
              <span>About Me</span>
            </a>
          </p>
          <p class="control">
            <a class="button is-black gradientbutton" href="#skills">
              <span>Skills</span>
            </a>
          </p>
          <p class="control">
            <a class="button is-black gradientbutton" href="#contact">
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
  margin-top: 4rem;
  color:white;
  font-family: "Prompt", sans-serif;
}


.gradientbutton {
  position: relative;
  font-family: inherit;
  font-weight: 500;
  letter-spacing: 0.05em;
  border-radius: 0.8em;
  border: none;
  background: linear-gradient(to right, #8e2de2, #4a00e0);
  color: ghostwhite;
  overflow: hidden;
  width: 10rem;
  font-family: "Prompt", sans-serif;
  width: 10rem;;
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

</style>