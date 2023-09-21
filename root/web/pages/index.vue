<template>
  <div class="flex flex-wrap justify-center items-center gap-1 mt-2 w-full h-auto">
    <CircleComponent :gap="4" />
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
