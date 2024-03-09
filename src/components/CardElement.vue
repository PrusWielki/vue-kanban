<script setup lang="ts">
defineProps({
  title: String,
  description: String
})
</script>
<template>
  <div class="container">
    <h1 class="title">{{ title }}</h1>
    <p>{{ description }}</p>
  </div>
</template>

<style scoped>
.container {
  width: 80%;
  display: flex;
  flex-direction: column;
  border: solid 1px black;
  border-radius: 90px;
  justify-content: start;
  align-items: center;
  height: fit-content;
}
.title {
  font-size: var(--font-lg);
  color: black;
}
</style>
