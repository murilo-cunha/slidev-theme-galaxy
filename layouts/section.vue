<script setup lang="ts">
import LayoutFooter from '../components/LayoutFooter.vue';
</script>

<template>
  <div class="slidev-layout section">
    <slot />
  </div>
  <LayoutFooter />
</template>