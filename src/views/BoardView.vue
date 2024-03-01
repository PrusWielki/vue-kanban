<script setup lang="ts">
import BoardElement from '@/components/BoardElement.vue'
import CardElement from '@/components/CardElement.vue'
</script>

<template>
  <div class="wrapper">
    <div class="container">
      <div class="board-grid">
        <BoardElement title="TODO"><CardElement title="Task1" /></BoardElement>
        <BoardElement title="Doing" />
        <BoardElement title="Done" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.wrapper {
  width: 100vw;
  height: 100lvh;
  background-color: var(--main-background);
}
.container {
  width: 100%;
  height: 100%;
  margin: 0 auto;
}
.board-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  width: 100%;
  height: 100%;
  column-gap: var(--gap-sm);
}
.table {
  width: 100%;
  height: 100%;
  background-color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: var(--padding-sm);
}
.table:hover {
  background-color: red;
}
</style>
