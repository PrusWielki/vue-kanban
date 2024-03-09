<script setup lang="ts">
defineProps({
  title: String
})
</script>
<template>
  <div class="container">
    <h1 class="title">{{ title }}</h1>
    <slot/>
  </div>
</template>

<style scoped>
.container {
  width: 100%;
  height: 100%;
  background-color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: var(--padding-sm);
}
.title {
  font-size: var(--font-lg);
  color: black;
}
</style>
