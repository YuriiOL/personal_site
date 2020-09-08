<template>
  <div class="stage" style="width: 220px; height: 220px;">
    <h1>Skills</h1>
    <div class="cubespinner">
      <div class="face1">
        <i class="fab fa-html5"></i>
      </div>
      <div class="face2">
        <i class="fab fa-css3-alt"></i>
      </div>
      <div class="face3">
        <i class="fab fa-js"></i>
      </div>
      <div class="face4">
        <i class="fab fa-vuejs"></i>
      </div>
      <div class="face5">
        <i class="fab fa-bootstrap"></i>
      </div>
      <div class="face6">
        <i class="fab fa-github"></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style type="text/css" scoped>
@-webkit-keyframes spincube {
  from,
  to {
    -webkit-transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
  }
  16% {
    -webkit-transform: rotateY(-90deg);
  }
  33% {
    -webkit-transform: rotateY(-90deg) rotateZ(90deg);
  }
  50% {
    -webkit-transform: rotateY(-180deg) rotateZ(90deg);
  }
  66% {
    -webkit-transform: rotateY(-270deg) rotateX(90deg);
  }
  83% {
    -webkit-transform: rotateX(90deg);
  }
}

@keyframes spincube {
  from,
  to {
    -moz-transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
    -ms-transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
    transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
  }
  16% {
    -moz-transform: rotateY(-90deg);
    -ms-transform: rotateY(-90deg);
    transform: rotateY(-90deg);
  }
  33% {
    -moz-transform: rotateY(-90deg) rotateZ(90deg);
    -ms-transform: rotateY(-90deg) rotateZ(90deg);
    transform: rotateY(-90deg) rotateZ(90deg);
  }
  50% {
    -moz-transform: rotateY(-180deg) rotateZ(90deg);
    -ms-transform: rotateY(-180deg) rotateZ(90deg);
    transform: rotateY(-180deg) rotateZ(90deg);
  }
  66% {
    -moz-transform: rotateY(-270deg) rotateX(90deg);
    -ms-transform: rotateY(-270deg) rotateX(90deg);
    transform: rotateY(-270deg) rotateX(90deg);
  }
  83% {
    -moz-transform: rotateX(90deg);
    -ms-transform: rotateX(90deg);
    transform: rotateX(90deg);
  }
}

.cubespinner {
  -webkit-animation-name: spincube;
  -webkit-animation-timing-function: ease-in-out;
  -webkit-animation-iteration-count: infinite;
  -webkit-animation-duration: 12s;

  animation-name: spincube;
  animation-timing-function: ease-in-out;
  animation-iteration-count: infinite;
  animation-duration: 12s;

  -webkit-transform-style: preserve-3d;
  -moz-transform-style: preserve-3d;
  -ms-transform-style: preserve-3d;
  transform-style: preserve-3d;

  -webkit-transform-origin: 60px 60px 0;
  -moz-transform-origin: 60px 60px 0;
  -ms-transform-origin: 60px 60px 0;
  transform-origin: 60px 60px 0;
}

.cubespinner div {
  position: absolute;
  width: 200px;
  height: 200px;
  border: 1px solid #ccc;
  background: rgba(255, 255, 255, 0.8);
  box-shadow: inset 0 0 20px rgba(0, 0, 0, 0.2);
  line-height: 180px;
  text-align: center;
  font-size: 100px;
  color: black;
}

.cubespinner .face1 {
  -webkit-transform: translateZ(100px);
  -moz-transform: translateZ(60px);
  -ms-transform: translateZ(60px);
  transform: translateZ(100px);
}
.cubespinner .face2 {
  -webkit-transform: rotateY(90deg) translateZ(100px);
  -moz-transform: rotateY(90deg) translateZ(60px);
  -ms-transform: rotateY(90deg) translateZ(60px);
  transform: rotateY(90deg) translateZ(100px);
}
.cubespinner .face3 {
  -webkit-transform: rotateY(90deg) rotateX(90deg) translateZ(100px);
  -moz-transform: rotateY(90deg) rotateX(90deg) translateZ(60px);
  -ms-transform: rotateY(90deg) rotateX(90deg) translateZ(60px);
  transform: rotateY(90deg) rotateX(90deg) translateZ(100px);
}
.cubespinner .face4 {
  -webkit-transform: rotateY(180deg) rotateZ(90deg) translateZ(100px);
  -moz-transform: rotateY(180deg) rotateZ(90deg) translateZ(60px);
  -ms-transform: rotateY(180deg) rotateZ(90deg) translateZ(60px);
  transform: rotateY(180deg) rotateZ(90deg) translateZ(100px);
}
.cubespinner .face5 {
  -webkit-transform: rotateY(-90deg) rotateZ(90deg) translateZ(100px);
  -moz-transform: rotateY(-90deg) rotateZ(90deg) translateZ(60px);
  -ms-transform: rotateY(-90deg) rotateZ(90deg) translateZ(60px);
  transform: rotateY(-90deg) rotateZ(90deg) translateZ(100px);
}
.cubespinner .face6 {
  -webkit-transform: rotateX(-90deg) translateZ(100px);
  -moz-transform: rotateX(-90deg) translateZ(60px);
  -ms-transform: rotateX(-90deg) translateZ(60px);
  transform: rotateX(-90deg) translateZ(100px);
}
.stage {
  margin-top: -15%;
  margin-left: 40%;
}
h1 {
  margin-bottom: 25%;
  margin-left: 10%;
}
@media (max-width: 1300px) {
  .stage {
    margin-top: -15%;
    margin-left: 20%;
  }
}
@media (max-width: 1000px) {
  .stage {
    margin-top: -10%;
    margin-left: 20%;
  }
}
@media (max-width: 670px) {
  .stage {
    margin-top: 140%;
    margin-left: -100%;
  }
}
@media (max-height: 666px) {
  .stage {
    margin-top: 50%;
    margin-left: -80%;
  }
}
</style>

