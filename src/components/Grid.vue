<template>
  <div class="grid-container">
    <template v-for="row in 6">
      <div v-for="col in 6" :key="`${row}-${col}`" class="cell">hello</div>
    </template>
  </div>
</template>

<style scoped>
.grid-container {
  border: 1px solid black;
  display: grid;
  grid-template-columns: repeat(6, 100px);
  grid-template-rows: repeat(6, 40px);
  gap: 0;
}

.cell {
  border: 1px solid black;
  padding: 4px;
}
</style>
