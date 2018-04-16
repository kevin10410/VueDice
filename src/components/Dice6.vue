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
  transform: rotateX(690deg) rotateY(945deg) rotateZ(1170deg);
  position: relative;
  animation: row 2s linear normal;
}

@keyframes row {
  0% {
    transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg) translateZ(100px);
  }
  20%{
    transform: rotateX(915deg) rotateY(270deg) rotateZ(900deg) translateZ(100px);
  }
  60%{
    transform: rotateX(1500deg) rotateY(630deg) rotateZ(1260deg) translateZ(100px);
  }
  100% {
    transform: rotateX(1770deg) rotateY(945deg) rotateZ(1530deg) translateZ(0px);
  }
}
</style>
