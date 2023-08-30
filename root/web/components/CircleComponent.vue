<template>
  <ClientOnly>
    <div v-for="n in numberOfCircles" :key="n" class="rounded-full bg-blue-600 h-10 w-10"></div>
  </ClientOnly>
</template>

<script setup lang="ts">
  const { width: windowWidth, height: windowHeight } = useWindowSize();

  const windowArea = computed(() => windowHeight.value * windowWidth.value);

  const radius = computed(() => 40 / 2);
  const circleArea = computed(() => radius.value ** 2 * Math.PI);
  const numberOfCircles = computed(() => Math.ceil(windowArea.value / circleArea.value));

  onMounted(() => {
    console.log(numberOfCircles.value);
  });
</script>

<style scoped></style>
