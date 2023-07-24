<template>
  <nav class="navbar">
    <div class="nametitle" id="#top"><a href="#top">Laviele Trias</a></div>
    <div :class="['navbar-menu', { 'is-active': isNavbarActive }]">
      <div class="navbarlinks">
        <ul>
          <li><a href="#aboutpage">About Me</a></li>
          <li><a href="#education">Education</a></li>
          <li><a href="#skills">Skills</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#contact">Contact Me</a></li>
        </ul>
      </div>
    </div>
    <!-- <a
      role="button"
      class="navbar-burger burger"
      aria-label="menu"
      aria-expanded="false"
      data-target="navbarBasicExample"
      @click="toggleNavbar"
    >
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a> -->
  </nav>
  <div class="landingpage" id="top">
    <div class="landingpagewrap">
      <h1>Hello, world.</h1>
      <h2>My name is Laviele Trias. I am an aspiring software developer.</h2>
      <button class="gradientbutton">
        <span><a href="#contact">Contact Me</a></span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
    // data() {
    //   return {
    //     isNavbarActive: false,
    //   };
    // },
    // methods: {
    //   toggleNavbar() {
    //     this.isNavbarActive = !this.isNavbarActive;
    //   },
    // },
};
</script>

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
  position: sticky;
  top: 0;
  left: 0;
  right: 0;
  width: 100%;
  z-index: 999;
}

.nametitle {
  font-size: 1.5rem;
  margin: 2rem;
  cursor: pointer;
}

.navbarlinks ul {
  margin: 0;
  padding: 0;
  display: flex;
  cursor: pointer;
}

.navbarlinks li {
  list-style: none;
}

.navbarlinks li a {
  text-decoration: none;
  color: white;
  padding: 1rem;
  display: block;
}

.navbarlinks li :hover {
  background-image: linear-gradient(144deg, #af40ff, #5b42f3 50%, #00ddeb);
}

.landingpage {
  display: flexbox;
  justify-content: space-between;
  align-items: center;
  background: url(../assets/homebg.jpg) no-repeat;
  background-size: cover;
  height: 100vh;
  flex-direction: column;
}

/* Landing Page */
.landingpagewrap {
  font-family: "Roboto", sans-serif;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  color: white;
}

.landingpage h1 {
  margin-bottom: 10px;
  align-items: left;
  font-size: 100px;
  background: -webkit-linear-gradient(144deg, #af40ff, #5b42f3 50%, #00ddeb);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-family: "Prompt", sans-serif;
}

.landingpage h2 {
  gap: 0;
  align-items: left;
  font-size: 25px;
  font-family: "Palanquin", sans-serif;
}

/* Gradient Buttons */

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
</style>
