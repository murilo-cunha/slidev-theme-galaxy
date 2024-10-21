<script setup lang="ts">
import TwoCols from './two-cols.vue';

const props = defineProps({
  class: {
    type: String,
  },
  layoutClass: {
    type: String,
  },
})
</script>

<template>
  <TwoCols :class="props.class" :layout-class="props.layoutClass">
    <template v-slot>
      <slot />
    </template>
    <template v-slot:left>
      <slot name="left" />
    </template>
    <template v-slot:right>
      <slot name="right" />
    </template>
    <template v-slot:bottom>
      <slot name="bottom" />
    </template>
  </TwoCols>
</template>