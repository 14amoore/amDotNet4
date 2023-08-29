<template>
  <div class="flex flex-wrap gap-1 w-full h-auto">
    <CircleComponent />
  </div>
</template>

<script setup lang="ts">
  interface Testing {
    name: string;
    id: number;
  }
  const testObj: Testing = {
    name: 'Adam Moore',
    id: 1,
  };
</script>

<style lang="scss" scoped></style>
