<template>
  <div class="bannertext-container">
    <h1>
      <span class="name">YOU SU JUNG</span>
      <span class="job"><br />FRONTEND</span>
    </h1>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.bannertext-container {
  display: flex;
  align-items: center;
  justify-content: center;
}
h1 {
  display: flex;
  font-family: 'Rammetto One', cursive;
  font-size: 6vw;
  letter-spacing: 3px;
}
.job {
  position: relative;
  color: rgb(255, 115, 150);
  align-self: flex-end;
}
.name {
  position: relative;
  align-self: flex-start;
}
.name::after {
  content: '|';
  position: absolute;
  right: 0;
  width: 100%;
  color: black;
  background: rgb(244, 224, 109);
  animation: typing 1.2s steps(11) forwards, caret 1s infinite;
}
.job::after {
  content: '|';
  position: absolute;
  right: 0;
  width: 100%;
  color: rgb(255, 115, 150);
  background: rgb(244, 224, 109);
  animation: typing 0.8s 1.2s steps(8) forwards, caret 1s infinite;
}
@keyframes typing {
  to {
    width: 0;
  }
}
@keyframes caret {
  50% {
    color: transparent;
  }
}
</style>
