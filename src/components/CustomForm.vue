<template>
  <div class="custom">
    <span class="work">I want to work for</span>
    <div class="box1"></div>
    <span class="minutes1">minutes.</span>
    <div class="arrow"></div>
    <span class="break">Then break for</span>
    <div class="box2"></div>
    <span class="minutes2">minutes.</span>
    <div class="arrow"></div>
  </div>
</template>

<script>
export default {
  name: 'CustomForm',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .custom{
    height: 100%;
    display: grid;
    grid-template-columns: repeat(9, 1fr);
    grid-template-rows: repeat(6, 1fr);
    grid-gap: 3px;
    text-align: center;
    font-size: 12px;
  }
  .work {
    grid-column: 2/6;
    grid-row: 2;
    font-size: 12px;
    margin: auto;
  }
  .box1 {
    grid-column: 6;
    grid-row: 2;
    background-color: grey;
    margin: 0px 2px 8px 2px;
  }
  .minutes1 {
    grid-column: 7/8;
    grid-row: 2;
    font-size: 12px;
    margin: auto;
  }
  .break {
    grid-column: 2/6;
    grid-row: 3;
    font-size: 12px;
    margin: auto;
  }
  .box2 {
    grid-column: 6;
    grid-row: 3;
    background-color: grey;
    margin: 0px 2px 8px 2px;
  }
  .minutes2 {
    grid-row: 3;
    grid-column: 7/8;
    font-size: 12px;
    margin: auto;
  }
  .arrow {

  }


</style>
