<template>
  <div class="section" id="contact">
    <div class="skills">
      <div class="title is-size-1 has-text-left">Contact Me</div>
      <div class="contactcard">
        <div class="contactcard-content has-text-left">
          <div class="contactdetails">
            <div class="contactabout-text">
              <p>Email: lstrias@up.edu.ph</p>
              <p>Phone Number: +639287616596</p>
              <p>Reach out to me on Social Media Below!</p>

              <div class="buttonwrap">
                <button class="gradientbutton" @click="redirectToFacebook">
                  <span>Facebook</span>
                </button>

                <button class="gradientbutton" @click="redirectToTwitter">
                  <span>Twitter</span>
                </button>

                <button class="gradientbutton" @click="redirectToInstagram">
                  <span>Instagram</span>
                </button>

                <button class="gradientbutton" @click="redirectToLinkedIn">
                  <span>LinkedIn</span>
                </button>

                <button class="gradientbutton" @click="redirectToGithub">
                  <span>Github</span>
                </button>
              </div>
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
    redirectToFacebook() {
      window.location.href = "https://www.facebook.com/vielle.trias";
    },

    redirectToTwitter() {
      window.location.href = "https://twitter.com/lxviele";
    },

    redirectToInstagram() {
      window.location.href = "https://www.instagram.com/lxviele/";
    },
    redirectToLinkedIn() {
      window.location.href =
        "https://www.linkedin.com/in/laviele-trias-3630911b9/";
    },
    redirectToGithub() {
      window.location.href = "https://github.com/Alunxina";
    },

    // Add more methods for other social media buttons as needed
  },
};
</script>

<style lang="scss" scoped>
@import "~bulma/css/bulma.css";

/*Contacts Card Display*/

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
  margin-left: 10rem;
}

.contactcard {
  width: 80%;
  height: auto;
  border-radius: 20px;
  padding: 5px;
  box-shadow: rgba(151, 65, 252, 0.2) 0 15px 30px -5px;
  background-image: linear-gradient(144deg, #af40ff, #5b42f3 50%, #00ddeb);
  margin-left: 8%;
  margin-bottom: 10%;
}

.contactcard-content {
  background: rgb(5, 6, 45);
  border-radius: 17px;
  width: 100%;
  height: 100%;
  padding-top: 3rem;
}

.contactabout-text {
  width: auto;
  margin-left: 1rem;
  margin-right: 1rem;
}

.contactabout-text h2 {
  font-size: 70px;
  margin-bottom: 20px;
  margin-top: 100px;
  font-family: "Prompt", sans-serif;
  background: -webkit-linear-gradient(144deg, #af40ff, #00ddeb 50%, #5b42f3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.contactabout-text h5 {
  letter-spacing: 2px;
  font-size: 80px;
  margin-bottom: 25px;
  margin-top: 20px;
  margin-left: 5rem;
  color: white;
  font-family: "Prompt", sans-serif;
}

.contactabout-text p {
  color: white;
  letter-spacing: 1px;
  font-size: 20px;
  margin-bottom: 40px;
  font-family: "Prompt", sans-serif;
  margin-left: 5rem;
  width: auto;
}

.buttonwrap {
  margin-left: 5rem;
  align-items: center;
  justify-content: space-around;
  padding-bottom: 3rem;
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

/* Mobile responsive layout using Bulma classes */
@media screen and (max-width: 768px) {
  .contactcard {
    width: 95%;
    margin-left: 2.5%;
  }

  .contactabout-text h2 {
    font-size: 40px;
    margin-top: 50px;
  }

  .contactabout-text h5 {
    font-size: 40px;
    margin-left: 2.5rem;
  }

  .contactabout-text p {
    font-size: 16px;
    margin-left: 2.5rem;
  }

  .buttonwrap {
    margin-left: 2.5rem;
  }
}
</style>
