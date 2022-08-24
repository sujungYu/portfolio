<template>
  <div class="a">
    <content-box>
      <project-num>팀 프로젝트(2명)</project-num>
      <used-tech>vue</used-tech>
      <used-tech>vuex</used-tech>
      <used-tech>vue-router</used-tech>
      <used-tech>eslint</used-tech>
      <used-tech>prettier</used-tech>
      <used-tech>vue-router</used-tech>
      <used-tech>vue2-datepicker</used-tech>
      <used-tech>sockjs-client</used-tech>
      <used-tech>webstomp-client</used-tech>
      <span>2021.04.01~2021.04.05</span>
      <div class="box">
        <!-- 모달창으로 변경 -->
        <!-- <div class="image-container">
          <img :src="image" />
          <div>
            <i class="fa-solid fa-angle-left" @click="pre"></i>
            {{ num }} / 2
            <i class="fa-solid fa-angle-right" @click="post"></i>
          </div>
        </div> -->
        <div class="text-container">
          <h2>3355 웹앱</h2>
          <h3>
            <ul>
              <li>
                <i class="fa-solid fa-check"></i> 지역별 스터디를 제공하기 위해
                개발
              </li>
              <li>
                <i class="fa-solid fa-check"></i>백엔드 1명, 프론트엔드 1명이서
                진행한 프로젝트로 디자인과 프론드엔드를 담당
              </li>
              <li><i class="fa-solid fa-check"></i>figma로 스토리보드 작성</li>
              <li>
                <i class="fa-solid fa-check"></i>vuex를 활용해 컴포넌트 간에
                통신이나 데이터를 효율적으로 전달하도록 구현
              </li>
              <li>
                <i class="fa-solid fa-check"></i> sockjs-client와
                webstomp-client를 활용해 채팅 구현
              </li>
              <li>
                <i class="fa-solid fa-check"></i>ESLint를 활용해 코드를 일관성
                있게 작성
              </li>
              <li>
                <i class="fa-solid fa-check"></i> Prettier을 활용해 코드스타일을
                일관되게 유지
              </li>
              <li>
                <i class="fa-solid fa-check"></i>vue-router을 활용하여 SPA 구현
              </li>
              <li>
                <i class="fa-solid fa-check"></i>vue2-datepicker를 활용해 스터디
                기간 구현
              </li>
              <li>
                <i class="fa-solid fa-check"></i> 요청, 응답만 받는 api를
                분리하여 작성
              </li>
              <li>
                <i class="fa-solid fa-check"></i> 코드 스플리팅을 활용해 페이지
                로딩 속도를 개선
              </li>
              <li><i class="fa-solid fa-check"></i>views___</li>
              <!-- <li><i class="fa-solid fa-check"></i>open api, momnet 사용</li> -->
            </ul>
          </h3>
          <i class="fa-brands fa-github"></i>
          <i class="fa-solid fa-globe"></i>
          <i class="fa-solid fa-camera"></i>
        </div>
      </div>
    </content-box>
  </div>
</template>

<script>
import ContentBox from './common/ContentBox.vue';
import ProjectNum from './common/ProjectNum.vue';
import UsedTech from './common/UsedTech.vue';
export default {
  components: {
    ContentBox,
    UsedTech,
    ProjectNum,
  },
  data() {
    return {
      num: 1,
      covid1: require('../assets/images/covid1.png'),
      covid2: require('../assets/images/covid2.png'),
    };
  },
  computed: {
    image() {
      if (this.num == 1) {
        return this.covid1;
      } else {
        return this.covid2;
      }
    },
  },
  methods: {
    pre() {
      return (this.num = 1);
    },
    post() {
      return (this.num = 2);
    },
  },
};
</script>

<style scoped>
.a {
  position: relative;
}
.content-container {
  margin-left: 8vw;
  padding: 3vh 3vw;
  /* position: absolute; */
  /* top: 1vh;
  left: 1vw; */
}
.box {
  display: flex;
  width: 100%;
  height: 100%;
}
/* .image-container {
  width: 40%;
}
.text-container {
  width: 70%;
} */
img {
  width: 100%;
}
ul li {
  list-style: none;
  /* padding: 0; */
}
ul {
  padding: 0;
}
</style>
