<template>
  <div class="a">
    <content-box>
      <project-num>개인 프로젝트</project-num>
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
          <h2>news 웹</h2>
          <h3>
            <ul>
              <li>
                <i class="fa-solid fa-check"></i> 요청, 응답만 받는 api를
                분리하여 작성
              </li>
              <li>
                <i class="fa-solid fa-check"></i> Async&Await를 활용해 비동기
                처리 문제 해결
              </li>
              <li>
                <i class="fa-solid fa-check"></i> 이벤드 버스를 활용해 스피너
                구현
              </li>
              <li>
                <i class="fa-solid fa-check"></i> Mixin을 활용해 컴포넌트 간에
                공통으로 사용하고 있는 로직을 재사용
              </li>
              <li>
                <i class="fa-solid fa-check"></i> 네비게이션 가드를 활용해 특정
                페이지에 접근 제한
              </li>
              <li><i class="fa-solid fa-check"></i> vuex 모듈화</li>
              <li>
                <i class="fa-solid fa-check"></i> 라우터 트랜지션을 활용해
                템플릿에 효과 부여
              </li>
              <li>
                <i class="fa-solid fa-check"></i> vuex 헬퍼 함수를 활용해 코드
                간단화
              </li>
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
