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
  height: 20%;
  background-color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: var(--padding-sm);
  gap: var(--gap-md)
}
.title {
  font-size: var(--font-xl);
  color: black;
  font-weight: 700;
}
</style>
