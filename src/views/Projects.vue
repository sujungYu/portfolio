<template>
  <div>
    <head-line>PROJECTS</head-line>
    <!-- <div class="covid-container">
      <covid-project></covid-project>
    </div> -->
    <div>
      <offco-project></offco-project>
    </div>
    <!-- <div>
      <t-f-project></t-f-project>
    </div>
    <div>
      <news-project></news-project>
    </div> -->
  </div>
</template>

<script>
import HeadLine from '../components/common/HeadLine.vue';
// import CovidProject from '../components/CovidProject.vue';
// import NewsProject from '../components/NewsProject.vue';
import OffcoProject from '../components/OffcoProject.vue';
// import TFProject from '../components/TFProject.vue';
export default {
  components: {
    HeadLine,
    // CovidProject,
    OffcoProject,
    // TFProject,
    // NewsProject,
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
