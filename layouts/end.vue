<script setup lang="ts">
import LayoutFooter from '../components/LayoutFooter.vue';
</script>

<template>
  <div class="slidev-layout end">
    <slot>END</slot>
  </div>
  <LayoutFooter />
</template>

<style scoped lang="postcss">
.slidev-layout.end {
  @apply text-white text-opacity-85 text-xl tracking-widest bg-black h-full text-center grid place-content-center select-none;
}
</style>