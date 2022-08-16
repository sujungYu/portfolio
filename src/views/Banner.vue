<template>
  <div class="banner-container">
    <banner-text></banner-text>
    <i class="fa-solid fa-circle-chevron-down down"></i>
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
  top: 90%;
  font-size: 4rem;
}
</style>
