<script setup lang="ts">
defineProps({
  title: String
})
</script>
<template>
  <div class="container">
    <h1 class="title">{{ title }}</h1>
  </div>
</template>

<style scoped>
.container {
  width: 80%;
  display: flex;
  flex-direction: column;
  border: solid 1px;
  border-radius: 90px;
}
.title {
  font-size: var(--font-sm);
  color: black;
}
</style>
