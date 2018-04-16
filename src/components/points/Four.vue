<template>
  <div>
      <div class="panel four">
          <div class="dot1">

          </div>
          <div class="dot2">
              
          </div>
          <div class="dot3">
              
          </div>
          <div class="dot4">
              
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

.four{
    transform: rotateY(180deg) translateZ(100px);
}

.dot1 {
  position: absolute;
  top: 25px;
  left: 25px;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: red;
}

.dot2 {
  position: absolute;
  bottom: 25px;
  right: 25px;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: red;
}

.dot3 {
  position: absolute;
  top: 25px;
  right: 25px;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: red;
}

.dot4 {
  position: absolute;
  bottom: 25px;
  left: 25px;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: red;
}
</style>