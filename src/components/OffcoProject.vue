<template>
  <div class="a">
    <content-box>
      <project-num>팀 프로젝트(2명)</project-num>
      <used-tech>vue</used-tech>
      <used-tech>vuex</used-tech>
      <used-tech>vue-router</used-tech>
      <!-- <used-tech>moment.js</used-tech>
      <used-tech>vue-chartjs</used-tech>
      <used-tech>vue-router</used-tech> -->
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
          <h2>offco 웹앱</h2>
          <h3>
            <ul>
              <li>
                <i class="fa-solid fa-check"></i> 기존 sns의 단점을 보완한
                단체모임 sns을 제공하기 위해 개발
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
              <li><i class="fa-solid fa-check"></i>__을 활용해 캘린더 구현</li>
              <li>
                <i class="fa-solid fa-check"></i> localStorage를 이용해 로그인
                유지 기능 구현
              </li>
              <li>
                <i class="fa-solid fa-check"></i> Math.random()함수로 난수를
                생성하여 초대 링크 구현
              </li>
              <li>
                <i class="fa-solid fa-check"></i> 기능 별로 store을 모듈화하여
                분리해서 관리
              </li>
              <li>
                <i class="fa-solid fa-check"></i>vue-router을 활용하여 SPA 구현
              </li>
              <!-- <li><i class="fa-solid fa-check"></i>open api, momnet 사용</li> -->
            </ul>
          </h3>
          <i class="fa-brands fa-github"></i>
          <i class="fa-solid fa-globe"></i>
          <i class="fa-solid fa-camera"></i>
        </div>
      </div>
      <h4>최근 업데이트일 2021.1.1</h4>
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
