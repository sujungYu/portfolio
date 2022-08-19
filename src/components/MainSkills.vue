<template>
  <div>
    <skills-form>
      <span slot="type">
        <h2>MAIN-SKILLS</h2>
      </span>
      <template slot="content">
        <li>
          <span class="text">HTML</span><img src="../assets/images/html.png" />
        </li>
        <li>
          <span class="text">CSS</span><img src="../assets/images/css.png" />
        </li>
        <li>
          <span class="text">JavaScript</span
          ><img src="../assets/images/javascript.png" />
        </li>
        <li>
          <span class="text">Typescript</span
          ><img src="../assets/images/typescript.png" />
        </li>
        <li>
          <span class="text">Scss</span><img src="../assets/images/sass.png" />
        </li>
        <li>
          <span class="text">Vue</span><img src="../assets/images/vue.png" />
        </li>
        <li>
          <span class="text">NodeJS</span
          ><img src="../assets/images/node-js.png" />
        </li>
        <li>
          <span class="text">GitHub</span
          ><img src="../assets/images/github.png" />
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
