<template>
  <div class="main-container">
    <div class="nav-container">
      <navbar></navbar>
    </div>
    <div class="sub-container">
      <div id="home" class="container">
        <banner></banner>
      </div>
      <div id="about" class="container color2">
        <introduce></introduce>
      </div>
      <div id="skill" class="container color1">
        <skills></skills>
      </div>
      <div id="project" class="container color2">
        <projects></projects>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Banner from './views/Banner.vue';
import Introduce from './views/Introduce.vue';
import Projects from './views/Projects.vue';
import Skills from './views/Skills.vue';
export default {
  components: {
    Navbar,
    Banner,
    Introduce,
    Skills,
    Projects,
  },
};
</script>

<style>
.main-container {
  width: 100vw;
}
.nav-container {
  z-index: 3;
  position: fixed;
  width: 100vw;
  height: 6vh;
  top: 0;
  left: 0;
}
.sub-container {
  position: relative;
  margin-top: 6vh;
}
.container {
  width: 100vw;
  height: 94vh;
  /* margin-bottom: 10vh; */
  /* background-color: rgb(255, 255, 222); */
}
.color1 {
  background-color: rgb(244, 224, 109);
}
.color2 {
  background-color: rgb(255, 255, 222);
}
</style>
