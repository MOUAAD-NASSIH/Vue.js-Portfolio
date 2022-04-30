<template>
  <div class="container">
    <NavBar />
    <Main />
    <Projects />
    <Technologies />
    <AboutMe />
    <Footer />
  </div>
</template>

<script>
import NavBar from "../components/NavBar.vue";
import Main from "../components/Main.vue";
import Projects from "../components/Projects.vue";
import Technologies from "../components/Technologies.vue";
import AboutMe from "../components/AboutMe.vue";
import Footer from "../components/Footer.vue";

export default {
  components: {
    NavBar,
    Main,
    Projects,
    Technologies,
    AboutMe,
    Footer,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
  scroll-behavior: smooth;
}

body {
  background: #0f1624;
}

.container {
  width: 80%;
  margin: 0 auto;
}
</style>
