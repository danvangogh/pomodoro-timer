<template>
  <form class="premade">
    <div class="break"></div>
    <div v-for="split in splits">{{ split[0] }} / {{ split[1] }}</div>
    <button
      class="start-btn"
      value="start"
      >Start</button>
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
    grid-column: 1/10;
    grid-row: 2/8;
    padding: 0 1em;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(6, 1fr);
    grid-gap: 3px;
    text-align: center;
  }
  .break {
    grid-column: 1/4;
  }
  .start-btn {
    grid-column: 1/4;
    width: 50%;
    height: 120%;
    margin: 1em auto auto auto;
    border: none;
    border-radius: 5px;
    background-color: #FF9501;
    color: #FFFFFF;
    font-size: 14px;
    line-height: 0px;
  }
</style>
