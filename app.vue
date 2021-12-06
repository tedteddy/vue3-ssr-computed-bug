<template>
  <div :style="style" />
</template>

<script lang="ts" setup>
import { computed } from "vue";

const style: any = computed(() => {
  if (process.client) {
    return {
      height: '200px',
      width: '200px',
      background: 'black',
    }
  }
  return {
    height: '100px',
    width: '100px',
    background: 'red',
  }
})

</script>
