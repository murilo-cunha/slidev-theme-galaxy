<script setup lang="ts">
import LayoutFooter from '../components/LayoutFooter.vue';
</script>

<template>
  <div class="slidev-layout statement">
    <div class="my-auto">
      <slot />
    </div>
  </div>
  <LayoutFooter />
</template>