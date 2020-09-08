<template>
  <div>
    <h1>I'm Yurii Oleksovskyi</h1>
    <span>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit.
      Quas itaque reiciendis sapiente ratione sit neque consequuntur odio?
      Corrupti, repudiandae commodi! Lorem ipsum dolor sit amet consectetur
      adipisicing elit. Quod maiores, deleniti sint tenetur sit laborum omnis
      sequi repellat aut voluptatum recusandae molestiae cupiditate quidem in
      vel quos. Aliquam, nobis consectetur!
    </span>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
div {
  width: 30%;
  height: 30%;
}
@media (max-width: 1000px) {
  div {
    width: 250px;
    margin-left: -15%;
    height: 40%;
  }
}
@media (max-width: 670px) {
  div {
    width: 300px;
    font-size: 15px;
    margin-left: -15%;
    height: 90%;
  }
}
@media (max-height: 666px) {
  div {
    width: 250px;
    font-size: 10px;
    margin-left: -15%;
    height: 100%;
  }
}
</style>
