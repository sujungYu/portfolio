<template>
  <div class="main-container">
    <div class="nav-container">
      <navbar></navbar>
    </div>
    <div class="sub-container">
      <div class="container">
        <banner></banner>
      </div>
      <div class="container">
        <introduce></introduce>
      </div>
      <div class="container">
        <skills></skills>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Banner from './views/Banner.vue';
import Introduce from './views/Introduce.vue';
import Skills from './views/Skills.vue';
export default {
  components: {
    Navbar,
    Banner,
    Introduce,
    Skills,
  },
};
</script>

<style>
.main-container {
  width: 100vw;
}
.nav-container {
  z-index: 1;
  position: fixed;
  width: 100vw;
  height: 6vh;
  top: 0;
  left: 0;
}
.sub-container {
  /* position: relative; */
  margin-top: 6vh;
}
.container {
  width: 100vw;
  height: 94vh;
}
</style>
