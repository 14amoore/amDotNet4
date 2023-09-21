<template>
  <ClientOnly>
    <div v-for="n in totalCircles" :key="n" class="rounded-full bg-blue-600 h-10 w-10"></div>
  </ClientOnly>
</template>

<script setup lang="ts">
  const { width: windowWidth, height: windowHeight } = useWindowSize();

  const props = defineProps({
    gap: {
      required: true,
      type: Number,
    },
  });

  const circleSize = 40 + props.gap;

  const horizontalMax = computed(() => Math.floor(windowWidth.value / circleSize));
  const verticalMax = computed(() => Math.floor(windowHeight.value / circleSize));
  const totalCircles = computed(() => horizontalMax.value * verticalMax.value);
</script>

<style scoped></style>
