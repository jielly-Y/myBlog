<template>
  <div id="app">
    <Layout>
      <template #left>
        <div class="aside"><SiteAside /></div>
      </template>
      <template #default>
        <RouterView />
      </template>
    </Layout>
  </div>
</template>

<script>
import Layout from "./components/Layout";
import SiteAside from "./components/SiteAside";
export default {
  components: {
    Layout,
    SiteAside,
  },
};
</script>

<style scoped lang="less">
@import "./styles/common.module.less";
#app {
  .self-fill(fixed);
}
.aside {
  width: 250px;
  height: 100%;
}
</style>
