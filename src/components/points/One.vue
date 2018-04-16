<template>
  <div>
      <div class="panel one">
          <div class="center">
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

.one{
    transform: rotateY(0) translateZ(100px);
}

.center {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    background: red;
}
</style>

