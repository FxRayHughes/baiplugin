<script setup lang="ts">
import { CSSProperties } from 'vue';
import BHeader from "@/views/Home/BHeader.vue";
import BContent from "@/views/Home/BContent.vue";
const headerStyle: CSSProperties = {
  height: 64,
  paddingInline: 50,
  lineHeight: '64px',
  width: '100%',
  backgroundColor: '#ffffff',
  "border-bottom": "1px solid #e8e8e8"
};

const contentStyle: CSSProperties = {
  backgroundColor: '#ffffff',
};

const footerStyle: CSSProperties = {
  backgroundColor: '#ffffff',
};
</script>

<template>
  <a-space direction="vertical" :style="{ width: '100%' }" :size="[0, 48]">
    <a-layout>
      <a-layout-header :style="headerStyle">
        <b-header></b-header>
      </a-layout-header>
      <a-layout-content :style="contentStyle">
        <b-content></b-content>
      </a-layout-content>
      <a-layout-footer :style="footerStyle"></a-layout-footer>
    </a-layout>
  </a-space>
</template>

<style scoped>

</style>
