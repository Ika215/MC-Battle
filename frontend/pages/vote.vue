<script setup lang="ts">
definePageMeta({
  layout: 'default',
})

const isVoted = ref<boolean>(false)

const MC1 = "CHICO CARLITO"
const MC2 = "句潤"
</script>
<template>
  <PageTitle :title="MC1 + ' VS ' + MC2" />
  <BattleMovie />
  <VoteButton @voted="isVoted = true"/>
  <VoteResult v-if="isVoted" />
</template>