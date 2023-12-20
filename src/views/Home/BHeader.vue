<template>
  <a-flex id="head" justify="space-between">
    <div id="logo">
      <span id="logo-text">XiaoBaiCat</span>
    </div>
    <div id="logo">
      <a-button type="text">登录</a-button>
      <a-button type="primary">注册</a-button>
    </div>
  </a-flex>
</template>

<script setup lang="ts">
import type { CSSProperties } from 'vue';
</script>


<style scoped>
#logo-text{
  font-size: 25px;
  color: #1a1a1a;
  font-family: "HarmonyOS Sans Black",system-ui
}
#head{
  border-bottom: 1px solid #e8e8e8;
}

</style>
