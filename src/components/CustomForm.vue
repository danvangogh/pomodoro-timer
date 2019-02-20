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
    <div class="start-btn"></div>
  </div>
</template>

<script>
export default {
  name: 'CustomForm',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .work {
    grid-area: wr;
    font-size: 10px;
    margin: auto;
  }
  .box1 {
    grid-area: box1;
    background-color: grey;
    margin: 0px 2px 8px 2px;
  }
  .box2 {
    grid-area: box2;
    background-color: grey;
    margin: 0px 2px 8px 2px;
  }
  .minutes1 {
    grid-area: m1;
    font-size: 10px;
    margin: auto;
  }
  .minutes2 {
    grid-area: m2;
    font-size: 10px;
    margin: auto;
  }
  .arrow {

  }
  .break {
    grid-area: br;
    font-size: 10px;
    margin: auto;
  }
  .start-btn {
    text-align: center;
  }
</style>
