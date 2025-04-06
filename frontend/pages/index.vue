<script setup lang="ts">
import PageTitle from '~/components/PageTitle.vue';
import ToVoteLink from '~/components/vote/ToVoteLink.vue';

definePageMeta({
  layout: 'default',
})
</script>
<template>
  <div>
    <PageTitle title="トップページ" />
    <ToVoteLink url="/vote" name="CHICOCARLITO VS 句潤" />
  </div>
</template>