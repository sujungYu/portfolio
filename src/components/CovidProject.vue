<template>
  <div class="a">
    <project-num>개인 프로젝트</project-num>
    <content-box>
      <used-tech>vue</used-tech>
      <used-tech>node.js</used-tech>
      <used-tech>d3.js</used-tech>
      <used-tech>moment.js</used-tech>
      <used-tech>vue-chartjs</used-tech>
      <used-tech>vue-router</used-tech>
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
          <h2>코로나19 웹사이트</h2>
          <h3>
            <ul>
              <li>
                <i class="fa-solid fa-check"></i> 코로나19 관련 정보를 제공하기
                위해 개발
              </li>
              <li>
                <i class="fa-solid fa-check"></i>공공 데이터에서 제공하는 open
                api를 활용
              </li>
              <li>
                <i class="fa-solid fa-check"></i>
                moment를 이용해 날짜 변동에 따른 데이터 자동 업로드가 가능하도록
                구현
              </li>
              <li>
                <i class="fa-solid fa-check"></i>우리나라 topojoson 데이터를
                활용
              </li>
              <li>
                <i class="fa-solid fa-check"></i> d3를 활용해 데이터 시각화
              </li>
              <li>
                <i class="fa-solid fa-check"></i> vue-router을 이용해 시, 도별
                코로나 확진자 및 백신 접종자 확인 가능
              </li>
              <li>
                <i class="fa-solid fa-check"></i> vue-chartjs을 이용해 최근
                7일내 확진자를 한 눈에 볼 수 있도록 구현
              </li>
              <li>
                <i class="fa-solid fa-check"></i>xml-js를 이용해 xml 데이터를
                json으로 파싱
              </li>
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
