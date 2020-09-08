<template>
  <div class="wrapper">
    <h1>
      Hi!
      <br />I'm web developer Yura,
      <br />and my life is kinda crazy.
    </h1>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.wrapper {
  height: 30%;
  width: 100%;
}
@media (max-width: 1000px) {
  .wrapper {
    height: 50%;
  }
}
@media (max-width: 500px) {
  .wrapper {
    font-size: 10px;
    width: 500px;
  }
}
</style>
