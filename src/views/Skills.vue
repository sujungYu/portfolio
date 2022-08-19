<template>
  <div>
    <head-line>SKILLS</head-line>
    <div class="skills-container">
      <main-skills></main-skills>
      <etc-skills></etc-skills>
    </div>
  </div>
</template>

<script>
import HeadLine from '../components/common/HeadLine.vue';
import EtcSkills from '../components/EtcSkills.vue';
import MainSkills from '../components/MainSkills.vue';
export default {
  components: { HeadLine, MainSkills, EtcSkills },
};
</script>

<style scoped>
.skills-container {
  position: relative;
  top: 12vh;
  z-index: 0;
}
</style>
