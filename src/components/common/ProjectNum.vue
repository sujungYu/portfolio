<template>
  <div class="num-container">
    <slot> </slot>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.num-container {
  position: absolute;
  top: -3vh;
  left: 6vw;
  /* left: -7vw;
  top: -5vh; */
  /* left: -4vw;
  top: -3vh; */
  /* left: -3vw;
  top: -1vh; */
  /* position: absolute;
  top: 1vh;
  left: 1vw; */
  display: inline-block;
  border: 3px solid black;
  border-radius: 10px;
  background-color: white;
  transform: rotate(-10deg);
  font-size: 2rem;
  padding: 0.5vh 0.5vw;
  z-index: 1;
}
</style>
