<template>
  <div class="demo-button-row">
    <div class="demo-button-col">
      <t-button theme="primary"> 确定 </t-button>
      <t-button variant="outline"> 取消 </t-button>
    </div>
    <div class="demo-button-col">
      <t-button theme="primary"> 下一步 </t-button>
      <t-button variant="outline"> 上一步 </t-button>
    </div>
    <div class="demo-button-col">
      <t-button theme="primary"> 新建主机 </t-button>
      <t-button variant="outline"> 重装系统 </t-button>
      <t-button variant="outline"> 批量续费 </t-button>
      <t-button variant="outline">
        <template #icon>
          <more-icon />
        </template>
      </t-button>
    </div>
  </div>
</template>
<script>
import { MoreIcon } from 'tdesign-icons-vue-next';

export default {
  components: {
    MoreIcon,
  },
};
</script>
<style scoped>
.demo-button-row {
  display: flex;
}
.demo-button-col + .demo-button-col {
  margin-left: 32px;
}
.t-button + .t-button {
  margin-left: 16px;
}
</style>
