<template>
  <div class="wrapper">
    <AboutInfo></AboutInfo>
    <Triangle></Triangle>
    <div></div>
  </div>
</template>

<script>
import Triangle from "@/components/Triangle.vue";
import AboutInfo from "@/components/AboutInfo.vue";
export default {
  components: { AboutInfo, Triangle }
};
</script>

<style scoped>
</style>
