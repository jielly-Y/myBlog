<template>
  <div class="test-container">
    <Menu />
  </div>
</template>

<script>
import "@/styles/global.less";
import Menu from "./index.vue";
export default {
  components: {
    Menu,
  },
};
</script>

<style scoped lang="less">
.test-container {
  width: 400px;
  height: 600px;
  margin: 0 auto;
  background-color: #000;
  border: 2px solid red;
}
</style>
