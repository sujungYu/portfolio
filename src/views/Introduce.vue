<template>
  <div>
    <head-line>ABOUT ME</head-line>
    <div class="contentbox-container">
      <content-box>
        <introduce-text></introduce-text>
      </content-box>
    </div>
  </div>
</template>

<script>
import ContentBox from '../components/common/ContentBox.vue';
import HeadLine from '../components/common/HeadLine.vue';
import IntroduceText from '../components/IntroduceText.vue';
export default {
  components: { HeadLine, ContentBox, IntroduceText },
};
</script>

<style scoped>
.contentbox-container {
  position: relative;
  top: 6vh;
  z-index: -2;
}
</style>
