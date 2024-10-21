<script setup lang="ts">
import LinkedInIcon from './LinkedInIcon.vue';
import TwitterIcon from './TwitterIcon.vue';
</script>

<template>
  <footer
    class="bg-barBottom flex absolute w-full bottom-0 left-0 py-0.5 px-4 text-sm"
  >
    <div v-if="$slidev.nav.currentLayout !== 'intro'" class="w-1/3 text-left">
      <div v-if="!$slidev.configs.favicon.includes('slidevjs')" class="inline-block">
        <img :src="$slidev.configs.favicon" class="h-6 py-0.5 inline-block" />
      </div>
      <span v-if="$slidev.configs.title" class="px-2">{{
        $slidev.configs.title
      }}</span>
    </div>
    <div
      v-if="$slidev.nav.currentLayout !== 'intro'"
      class="w-2/3 flex justify-end"
    >
      <span v-if="$slidev.themeConfigs.linkedin" class="px-2">
        <LinkedInIcon strokeColor="rgb(241 245 249)" class="inline-block h-5" /> {{ $slidev.themeConfigs.linkedin }}
      </span>
      <span v-if="$slidev.themeConfigs.twitter" class="px-2">
        <TwitterIcon class="inline-block h-5" /> @{{ $slidev.themeConfigs.twitter }}
      </span>
      <span v-if="$slidev.themeConfigs.github" class="px-2">
        <GithubIcon class="inline-block h-5"/> @{{ $slidev.themeConfigs.github }}
      </span>
      <span v-if="$slidev.themeConfigs.showpages" class="px-2">
        {{ $slidev.nav.currentPage - 1 }} / {{ $slidev.nav.total - 1 }}
      </span>
    </div>
  </footer>
</template>
