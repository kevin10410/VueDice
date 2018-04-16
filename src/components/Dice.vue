<template>
  <div class="dice">
      <app-one></app-one>
      <app-two></app-two>
      <app-three></app-three>
      <app-four></app-four>
      <app-five></app-five>
      <app-six></app-six>
  </div>
</template>
<script>
import One from "./points/One.vue";
import Two from "./points/Two.vue";
import Three from "./points/Three.vue";
import Four from "./points/Four.vue";
import Five from "./points/Five.vue";
import Six from "./points/Six.vue";
export default {
  props:['point'],
  components: {
    appOne: One,
    appTwo: Two,
    appThree: Three,
    appFour: Four,
    appFive: Five,
    appSix: Six
  }
};
</script>
<style scoped>
.dice {
  width: 200px;
  height: 200px;
  margin: auto;
  /* background: yellow; */
  transform-style: preserve-3d;
  transform: rotateX(60deg) rotateY(0deg) rotateZ(45deg);
  position: relative;
  animation: row 6s ease-out infinite alternate;
}

@keyframes row {
  0% {
    transform: rotateX(60deg) rotateY(0deg) rotateZ(45deg);
  }
  20% {
    transform: rotateX(150deg) rotateY(45deg) rotateZ(360deg);
  }
  40% {
    transform: rotateX(330deg) rotateY(225deg) rotateZ(720deg);
  }
  60% {
    transform: rotateX(420deg) rotateY(540deg) rotateZ(945deg);
  }
  80% {
    transform: rotateX(510deg) rotateY(585deg) rotateZ(1170deg);
  }
  100%{
      transform: rotateX(690deg) rotateY(945deg) rotateZ(1170deg)
  }
}
</style>
