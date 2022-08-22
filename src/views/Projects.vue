<template>
  <div>
    <head-line>PROJECTS</head-line>
    <div class="covid-container">
      <covid-project></covid-project>
    </div>
  </div>
</template>

<script>
import HeadLine from '../components/common/HeadLine.vue';
import CovidProject from '../components/CovidProject.vue';
export default {
  components: {
    HeadLine,
    CovidProject,
  },
};
</script>

<style scoped>
.covid-container {
  position: relative;
  top: 13vh;
  margin-left: 0;
}
</style>
