<script setup lang="ts">
const props = defineProps({
  title: {
    type: String,
    required: true
  }
})
</script>
<template>
  <div>
    <h2>{{props.title}}</h2>
  </div>
</template>