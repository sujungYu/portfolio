<template>
  <div class="banner-container">
    <banner-text></banner-text>
    <a href="#about">
      <i class="fa-solid fa-circle-chevron-down down"></i>
    </a>
  </div>
</template>

<script>
import BannerText from '../components/BannerText.vue';
export default {
  components: { BannerText },
};
</script>

<style scoped>
.banner-container {
  position: relative;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: rgb(244, 224, 109);
}
.down {
  position: absolute;
  text-align: center;
  top: 80vh;
  font-size: 4rem;
}
a {
  color: black;
}
</style>
