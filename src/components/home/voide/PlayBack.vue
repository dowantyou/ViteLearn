<template>
  <div class="box">
    <div class="wifi-symbol">
      <div class="wifi-circle first"></div>
      <div class="wifi-circle second"></div>
      <div class="wifi-circle third"></div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.wifi-symbol {
  width: 50px;
  height: 50px;
  box-sizing: border-box;
  overflow: hidden;
  transform: rotate(135deg);
}

.wifi-circle {
  border: 5px solid #999999;
  border-radius: 50%;
  position: absolute;
}

.first {
  width: 5px;
  height: 5px;
  background: #cccccc;
  top: 45px;
  left: 45px;
}

.second {
  width: 25px;
  height: 25px;
  top: 35px;
  left: 35px;
  animation: fadeInOut 1s infinite 0.2s;
}

.third {
  width: 40px;
  height: 40px;
  top: 25px;
  left: 25px;
  animation: fadeInOut 1s infinite 0.4s;
}

@keyframes fadeInOut {
  0% {
    opacity: 0;
    /*初始状态 透明度为0*/
  }

  100% {
    opacity: 1;
    /*结尾状态 透明度为1*/
  }
}
</style>
