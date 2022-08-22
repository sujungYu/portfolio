<template>
  <div class="content-container">
    <slot></slot>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.content-container {
  position: relative;
  height: 90%;
  width: 50vw;
  margin: 0 auto;
  /* z-index: -2; */
  /* top: -4vh; */
  padding: 5vh 5vw;
  /* padding-bottom: 0; */
  /* display: flex; */
  /* align-items: center; */
  border: 3px solid black;
  border-radius: 15px;
  background-color: white;
}
</style>
