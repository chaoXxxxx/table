<template>
  <div>
    <rowSelectionVue />
    <rowSelectionAndOperationVue />
    <rowSelectionCustomVue />
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue';
import rowSelectionVue from './row-selection.vue';
import rowSelectionAndOperationVue from './row-selection-and-operation.vue';
import rowSelectionCustomVue from './row-selection-custom.vue';

export default defineComponent({
  components: {
    rowSelectionVue,
    rowSelectionAndOperationVue,
    rowSelectionCustomVue,
  },
  title: '可选择',
  enTitle: 'Selection',
  type: 'selection',
  children: [
    {
      id: 'row-selection',
      title: '可选择',
      enTitle: 'selection',
    },
    {
      id: 'row-selection-and-operation',
      title: '选择和操作',
      enTitle: 'Selection and operation',
    },
    {
      id: 'row-selection-custom',
      title: '自定义选择项',
      enTitle: 'Custom selection',
    },
  ],
  setup() {
    return {};
  },
});
</script>
<style lang="less" scoped></style>
