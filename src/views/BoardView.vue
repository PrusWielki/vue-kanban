<template>
  <div class="wrapper">
    <div class="container">
      <div class="board-grid">
        <div class="table">Hello</div>
        <div class="table">Hello</div>
        <div class="table">Hello</div>
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
