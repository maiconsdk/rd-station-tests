<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import 'https://d335luupugsy2.cloudfront.net/js/loader-scripts/43dd5f98-bea9-47d4-ad69-1058f5a37ed4-loader.js'
</script>

<template>
  <ul>
    <li><RouterLink to="/">Home</RouterLink></li>
    <li><RouterLink to="/about">About</RouterLink></li>
    <li><RouterLink to="/contact">Contact</RouterLink></li>
  </ul>
  <RouterView />
</template>

<style scoped>
</style>
