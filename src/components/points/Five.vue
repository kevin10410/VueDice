<template>
  <div>
      <div class="panel five">
          <div class="dot dot1">

          </div>
          <div class="dot dot2">
              
          </div>
          <div class="dot dot3">
              
          </div>
          <div class="dot dot4">

          </div>
          <div class="dot dot5">
              
          </div>
      </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.panel {
  width: 100%;
  height: 200px;
  background: rgba(255, 255, 255, 1);
  border-radius: 15px;
  border: 1px solid black;
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  top: 0;
  left: 0;
  backface-visibility: hidden;
}

.five {
  transform: rotateY(90deg) translateZ(100px);
}

.dot {
  position: absolute;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: black;
}

.dot1 {
  top: 25px;
  left: 25px;
}

.dot2 {
  bottom: 25px;
  right: 25px;
}

.dot3 {
  top: 25px;
  right: 25px;
}

.dot4 {
  bottom: 25px;
  left: 25px;
}

.dot5 {
  bottom: 75px;
  left: 75px;
}
</style>