<template>
  <div class="flex items-center justify-center rounded-full bg-red-600 w-24 h-24">
    <NuxtLink :to="route">{{ text }}</NuxtLink>
  </div>
</template>

<script setup lang="ts">
  defineProps({
    text: {
      required: true,
      type: String,
    },
    route: {
      required: true,
      type: String,
    },
  });
</script>

<style scoped></style>
