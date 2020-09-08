<template>
  <div class="wrapper">
    <HomeInfo></HomeInfo>
    <Logo></Logo>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeInfo from "@/components/HomeInfo.vue";
import Logo from "@/components/Logo.vue";
export default {
  name: "Home",
  components: { HomeInfo, Logo }
};
</script>
<style scoped>
.wrapper {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
</style>
