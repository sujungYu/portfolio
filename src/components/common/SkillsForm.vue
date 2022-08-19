<template>
  <div>
    <div class="type-container">
      <div class="type-display">
        <slot name="type"></slot>
      </div>
    </div>
    <content-box class="padding">
      <ul>
        <slot name="content"></slot>
      </ul>
    </content-box>
  </div>
</template>

<script>
import ContentBox from './ContentBox.vue';
export default {
  components: {
    ContentBox,
  },
};
</script>

<style scoped>
.padding {
  padding: 0;
}
.type-display {
  display: inline-block;
}
.type-container {
  width: 50vw;
  margin: 0 auto;
}
ul {
  padding: 0;
  list-style: none;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  /* grid-template-rows: repeat(4, 1fr); */
  text-align: center;
}
/* .container {
  width: 100%;
} */
</style>
