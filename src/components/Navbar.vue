<template>
  <div class="navbar-container">
    <nav>
      <ul>
        <li>YOUSUJUNG</li>
      </ul>
      <ul class="category-container">
        <li herf="#home">HOME</li>
        <li herf="#about">ABOUT</li>
        <li>SKILL</li>
        <li>PROJECT</li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.navbar-container {
  background-color: rgb(255, 249, 224);
  width: 100%;
  height: 100%;
}
nav {
  display: flex;
  justify-content: space-between;
}
ul {
  display: flex;
  list-style: none;
  letter-spacing: 2px;
  font-size: 1.3rem;
}
li {
  margin-right: 5vw;
  font-family: 'Signika Negative', sans-serif;
}
.category-container li:hover {
  font-weight: bolder;
  text-decoration: underline 1.2px;
  color: rgb(255, 115, 150);
}
</style>
