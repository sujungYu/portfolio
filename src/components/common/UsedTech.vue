<template>
  <div class="tech-container">
    <slot></slot>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.tech-container {
  display: inline-block;
  background-color: rgb(255, 115, 150);
  border-radius: 15px;
  color: white;
  font-size: 2rem;
  padding: 0 1vw;
  height: 4vh;
  line-height: 3.5vh;
}
</style>
