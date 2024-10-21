<script setup lang="ts">
import LayoutFooter from '../components/LayoutFooter.vue';
</script>

<template>
  <div class="slidev-layout default">
    <div class="my-auto w-full">
      <slot />
    </div>
  </div>
  <LayoutFooter />
</template>
