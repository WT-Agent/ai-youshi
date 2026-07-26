<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****5500 完成了中班科学《神奇的磁铁》公开课教案"
  },
  {
    "text": "用户 188****2211 获得了大班建构区合作搭城堡观察记录分析"
  },
  {
    "text": "用户 131****4499 完成了小班秋季环创“落叶色彩”区角方案"
  },
  {
    "text": "用户 153****7722 生成了解决小班分离焦虑家园共育指导书"
  },
  {
    "text": "用户 177****1133 取得了幼师半日活动流程与安全把控 Checklist"
  }
]);
</script>
