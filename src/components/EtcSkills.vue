<template>
  <div>
    <skills-form>
      <span slot="type">
        <h2>ETC.</h2>
      </span>
      <template slot="content">
        <li>
          <span class="text">Photoshop</span
          ><img src="../assets/images/photoshop.png" />
        </li>
        <li>
          <span class="text">Illust</span
          ><img src="../assets/images/illustrator.png" />
        </li>
        <li>
          <span class="text">Figma</span
          ><img src="../assets/images/figma.png" />
        </li>
        <li>
          <span class="text">MySQL</span
          ><img src="../assets/images/mysql.png" />
        </li>
      </template>
    </skills-form>
  </div>
</template>

<script>
import SkillsForm from './common/SkillsForm.vue';
export default {
  components: { SkillsForm },
};
</script>

<style scoped>
.text {
  display: block;
  font-family: 'Signika Negative', sans-serif;
  font-size: 1.6rem;
  /* border-bottom: 3px solid black; */
  margin: 1vh auto;
  font-weight: bold;
  /* text-align: center; */
}
img {
  height: 10vh;
  width: auto;
  /* width: 5vw;
  height: auto; */
}
h2 {
  width: 100%;
  white-space: nowrap;
  letter-spacing: 2.9px;
  font-size: 2em;
  font-family: 'Signika Negative', sans-serif;
  overflow: hidden;
  border-right: 3px solid;
  animation: typing 1s steps(11), blink 0.4s step-end infinite alternate;
}
@keyframes typing {
  from {
    width: 0%;
  }
}

@keyframes blink {
  50% {
    border-color: transparent;
  }
}
</style>
