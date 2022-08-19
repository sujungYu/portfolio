<template>
  <div class="button-container">
    <span class="text"><slot name="text"></slot></span>
    <span class="icon"><slot name="icon"></slot></span>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.button-container {
  position: relative;
  width: 50px;
  height: 50px;
}
/* .button-container {
  position: relative;
  font-size: 1.8rem;
  width: 50px;
  height: 50px;
  border: 2px solid rgb(255, 115, 150);
  border-radius: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
} */
.text {
  position: absolute;
  top: -5vh;
  z-index: -2;
  /* opacity: 0;/ */
}
.icon {
  position: relative;
  font-size: 1.8rem;
  width: 100%;
  height: 100%;
  border: 2px solid rgb(255, 115, 150);
  border-radius: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}
/* .icon:hover {
  color: red;
} */
/* .icon:hover .text {
  top: -45px;
  opacity: 2;
  visibility: visible;
  pointer-events: auto;
} */
.icon:hover .text {
  color: red;
  /* top: -45px; */
  z-index: 10;
  /* opacity: 1; */
  /* z-index: 2;
  opacity: 1; */
  /* visibility: visible; */
  /* pointer-events: auto; */
}
</style>
