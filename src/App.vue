<template>
  <div id="app">
    <HeaderComp />
    <div class="container">
      <router-view />
    </div>
  </div>
</template>
<script>
import HeaderComp from "./components/HeaderComp.vue";
export default {
  components: { HeaderComp },
};
</script>
<style lang="scss">
</style>
