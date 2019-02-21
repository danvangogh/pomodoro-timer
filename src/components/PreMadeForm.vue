<template>
  <form class="premade">
    <div class="break"></div>
    <div v-for="split in splits">{{ split[0] }} / {{ split[1] }}</div>
  </form>
</template>

<script>
export default {
  name: 'PreMadeForm',
  data() {
    return{
      splits: [
        [15, 3],
        [18, 4],
        [20, 5],
        [22, 6],
        [25, 7],
        [28, 8],
        [30, 9],
        [32, 10],
        [35, 11],
      ]
    }
  },
}
</script>

<style>
  .premade {
    padding: 0 2em;
    height: 60%;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(4, 1fr);
    grid-gap: 3px;
    text-align: center;
    font-size: 12px;
  }
  .break {
    grid-column: 1/4;
  }
</style>
