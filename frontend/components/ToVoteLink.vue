<script setup lang="ts">
const props = defineProps({
  url: {
    type: String,
    required: true
  },
  name: {
    type: String,
    required: true
  }
})
</script>
<template>
  <NuxtLink :to="props.url"> {{ props.name }} </NuxtLink>
</template>