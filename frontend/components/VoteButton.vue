<template>
  <div class="vote-button">
    <button class="vote-button__first" @click="$emit('voted')">先行</button>
    <button class="vote-button__second" @click="$emit('voted')">後攻</button>
  </div>
</template>

<style lang="scss" scoped>
.vote-button {
  &__first {
    margin-right: 20px;
  }
}
</style>
