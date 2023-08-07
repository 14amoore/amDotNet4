<template>
  <div>
    <h1 class="font-sans">Hi</h1>
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
