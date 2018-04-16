<template>
  <div>
      <div class="panel three">
          <div class="dot1">

          </div>
          <div class="dot2">
              
          </div>
          <div class="dot3">
              
          </div>
      </div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style scoped>
.panel{
    width: 100%;
    height: 200px;
    border-radius: 15px;
    background: #ffffff;
    border: 1px solid black;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    top: 0;
    left: 0;
    backface-visibility: hidden;
}

.three{
    transform: rotateX(90deg) translateZ(100px);
}

.dot1 {
  position: absolute;
  top: 25px;
  left: 25px;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: black;
}

.dot2 {
  position: absolute;
  bottom: 25px;
  right: 25px;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: black;
}

.dot3 {
  position: absolute;
  bottom: 75px;
  right: 75px;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: black;
}
</style>