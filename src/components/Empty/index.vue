<template>
  <div class="empty-container">
    <Icon type="empty" />
    <p>{{ text }}</p>
  </div>
</template>

<script>
import Icon from "@/components/Icon";
export default {
  components: {
    Icon,
  },
  props: {
    text: {
      type: String,
      default: "无数据",
    },
  },
};
</script>

<style scoped lang="less">
@import "~@/styles/common.module.less";
@import "~@/styles/var.less";
.empty-container {
  .abs-center();
  text-align: center;
  color: @gray;
}
.icon-container {
  font-size: 72px;
}
</style>
