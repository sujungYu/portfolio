<template>
  <div class="main-container">
    <div class="info-container">
      <img src="../assets/images/유수정.png" />
      <h3>유수정</h3>
      <h5>Frontend Developer</h5>
    </div>
    <div class="text-container">
      <h2>안녕하세요. <br />대화를 좋아하는 개발자 <br />유수정입니다.</h2>
      <h4>
        <p>
          프론트엔드 개발자는 여러 분야의 사람들과 함께 프로젝트를 진행하기
          때문에 대화가 중요하다고 생각합니다.
        </p>
        <p>
          원활한 대화를 하기 위해서는 다른 분야에 대한 이해가 필요하기 때문에,
          저는 분야를 가리지 않고 개발에 대한 관심사를 넓혀나가고 있습니다.
        </p>
      </h4>
      <div class="button-container">
        <info-button>
          <i slot="icon" class="fa-solid fa-phone"></i>
          <!-- <h1 slot="text">sdfsd</h1> -->
        </info-button>
        <info-button>
          <i slot="icon" class="fa-solid fa-envelope"></i>
          <!-- <h1 slot="text">sdfsd</h1> -->
        </info-button>
        <info-button>
          <i slot="icon" class="fa-brands fa-github"></i>
          <!-- <h1 slot="text">sdfsd</h1> -->
        </info-button>
        <info-button>
          <i slot="icon" class="fa-solid fa-b"></i>
          <!-- <h1 slot="text">sdfsd</h1> -->
        </info-button>
        <info-button>
          <i slot="icon" class="fa-solid fa-file"></i>
          <!-- <h1 slot="text">sdfsd</h1> -->
        </info-button>
      </div>
    </div>
  </div>
</template>

<script>
import InfoButton from './common/InfoButton.vue';
export default {
  components: { InfoButton },
};
</script>

<style scoped>
.main-container {
  display: flex;
  width: 100%;
  justify-content: space-between;
  font-family: 'Nanum Gothic', sans-serif;
}
.info-container {
  width: 30%;
}
.text-container {
  width: 50%;
}
h2,
h3,
h5 {
  text-align: center;
}
h2 {
  font-size: 2.9rem;
}
h3 {
  font-size: 2.6rem;
}
h4 {
  font-size: 1.7rem;
}
h5 {
  font-size: 1.4rem;
}
img {
  height: auto;
  width: 100%;
}
.button-container {
  display: flex;
}
</style>
