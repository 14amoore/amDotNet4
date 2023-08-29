<template>
  <div ref="pageSize" class="flex m-auto w-full h-full">
    <CircleComponent />
  </div>
</template>

<script setup lang="ts">
  const pageSize = ref(null);

  interface Testing {
    name: string;
    id: number;
  }
  const testObj: Testing = {
    name: 'Adam Moore',
    id: 1,
  };

  onMounted(() => {
    console.log(pageSize.value);
  });
</script>

<style lang="scss" scoped></style>
