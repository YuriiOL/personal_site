<template>
  <div>
    <div class="logWrapper">
      <div class="leftStick log"></div>
      <div class="rightStick log"></div>
      <div class="bottomStick"></div>
      <div class="endOfBottomStick"></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@media (max-width: 500px) {
  .logWrapper {
    display: none;
  }
}
.logWrapper {
  width: 200px;
  height: 370px;
  background-color: rgb(29, 29, 29);
  padding: 10px;
}
.leftStick {
  transform: matrix(1, 1.5, 0, 0.5, 0, 50);
}
.rightStick {
  transform: matrix(1, -1.5, 0, 0.5, 100, 50);
}

.endOfBottomStick {
  width: 21px;
  height: 22px;
  background-color: white;
  transform: translate(90px, 325px) rotate(47deg);
  position: absolute;
}
.bottomStick,
.rightStick,
.leftStick {
  width: 100px;
  height: 100px;
  background-color: white;
  position: absolute;
}
.bottomStick {
  width: 30px;
  height: 180px;
  transform: translate(85px, 156px);
}
.logWrapper:hover .leftStick {
  -webkit-box-shadow: 13px 4px 65px 12px rgba(255, 255, 255, 1);
  -moz-box-shadow: 13px 4px 65px 12px rgba(255, 255, 255, 1);
  box-shadow: 13px 4px 65px 12px rgba(255, 255, 255, 1);
}
.logWrapper:hover .rightStick {
  -webkit-box-shadow: -13px 4px 65px 12px rgba(255, 255, 255, 1);
  -moz-box-shadow: -13px 4px 65px 12px rgba(255, 255, 255, 1);
  box-shadow: -13px 4px 65px 12px rgba(255, 255, 255, 1);
}

.logWrapper:hover .endOfBottomStick {
  -webkit-box-shadow: -30px -23px 65px 12px rgba(252, 252, 252, 1);
  -moz-box-shadow: -30px -23px 65px 12px rgba(252, 252, 252, 1);
  box-shadow: -30px -23px 65px 12px rgba(252, 252, 252, 1);
}
.logWrapper:hover .bottomStick {
  -webkit-box-shadow: 0px 0px 39px 2px rgba(255, 255, 255, 1);
  -moz-box-shadow: 0px 0px 39px 2px rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 39px 2px rgba(255, 255, 255, 1);
}
</style>
