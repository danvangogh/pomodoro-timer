<template>
  <div class="premade">
    <span class="a">a</span>
  </div>
</template>

<script>
export default {
  name: 'PreMadeForm',
}
</script>

<style>
  .premade {
    grid-column: 1/10;
    grid-row: 2/8;
    background-color: purple;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(6, 1fr);
    grid-gap: 3px;
  }
</style>
