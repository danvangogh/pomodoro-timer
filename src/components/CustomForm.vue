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
    grid-column: 1/10;
    grid-row: 3/7;
    display: grid;
    grid-template-columns: repeat(9, 1fr);
    grid-template-rows: repeat(4, 1fr);
    grid-gap: 3px;
    text-align: center;
    font-size: 12px;
  }
  .work {
    grid-column: 2/6;
    font-size: 12px;
    margin: auto;
  }
  .box1 {

    background-color: grey;
    margin: 0px 2px 8px 2px;
  }
  .box2 {

    background-color: grey;
    margin: 0px 2px 8px 2px;
  }
  .minutes1 {
    grid-column: 7/9;
    font-size: 12px;
    margin: auto;
  }
  .minutes2 {
    grid-column: 7/9;
    font-size: 12px;
    margin: auto;
  }
  .arrow {

  }
  .break {
    grid-column: 2/6;
    font-size: 12px;
    margin: auto;
  }

</style>
