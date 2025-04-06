<script setup lang="ts">
import BattleMovie from '~/components/BattleMovie.vue'
import PageTitle from '~/components/PageTitle.vue'
import VoteButton from '~/components/vote/VoteButton.vue'
import VoteResult from '~/components/vote/VoteResult.vue'

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