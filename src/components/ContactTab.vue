<template>
  <footer class="footer">
    <div class="container">
    <div class="content has-text-centered">
      <div class="columns is-vcentered">
        <div class="column">
          <h1 class="title is-pulled-left">{{ contactTitle }}</h1>
        </div>
        <div class="column is-narrow">
          <div class="is-pulled-right">
            <a :href="emailLink">
              <img src="../assets/mail.png" alt="Email" width="50" height="50" style="padding-top: 15px;" >
            </a>
          </div>
        </div>
        <div class="column is-narrow">
          <div class="is-pulled-right">
            <a :href="linkedinLink">
              <img src="../assets/linkedin.png" alt="LinkedIn" width="50" height="50">
            </a>
          </div>
        </div>
        <div class="column is-narrow">
          <div class="is-pulled-right">
            <a :href="githubLink">
              <img src="../assets/github.png" alt="GitHub" width="50" height="50">
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      contactTitle: "Contact Me",
      emailLink: "mailto:lavieletrias12@gmail.com",
      linkedinLink: "https://www.linkedin.com/in/laviele-trias-3630911b9/",
      githubLink: "https://github.com/vieletrias",
    };
  },
};
</script>

<style lang="scss" scoped>
@import "~bulma/css/bulma.css";

.footer {
  background-color: #141416;
}
.title{
  padding-top:15px;
  font-family: "Prompt", sans-serif;
  color: white;
}

.footer{
  padding: 0.5rem 0.5rem 0.5rem 0.5rem;
}
</style>
