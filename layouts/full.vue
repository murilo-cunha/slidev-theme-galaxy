<script setup lang="ts">
import LayoutFooter from '../components/LayoutFooter.vue';
</script>

<template>
  <div class="slidev-layout full w-full h-full">
    <slot class="w-full h-full" />
  </div>
  <LayoutFooter />
</template>