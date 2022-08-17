<template>
  <div class="button-container">
    <span class="icon"><slot name="icon"></slot></span>
    <span class="text"><slot name="text"></slot></span>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.button-container {
  position: relative;
  font-size: 1.8rem;
  width: 50px;
  height: 50px;
  border: 2px solid rgb(255, 115, 150);
  border-radius: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.icon {
  position: relative;
}
.text {
  display: none;
}
.icon:hover .text {
  display: block;
}
</style>
