<template>
  <div class="clock">
    <div class="card">
      <span class="pre-made-split">Pre-made Splits</span>
      <span class="custom-split">Custom</span>
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
  </div>
</template>

<script>
export default {
  name: 'ClockSelection',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .clock {
    grid-area: cs;
    padding: 1em;
    color: white;
  }
  .card {
    margin: auto;
    width: 280px;
    height: 220px;
    border: 1px #707070 solid;
    border-radius: 5px;
    box-shadow: 1px 1px 1px #242424,
                2px 2px 1px #242424,
                3px 3px 1px #242424,
                4px 4px 1px #242424,
                5px 5px 0px #707070,
                6px 6px 1px #242424,
                7px 7px 1px #242424,
                8px 8px 1px #242424,
                9px 9px 1px #242424,
                10px 10px 0px #707070;
    display: grid;
    grid-template-columns: repeat(9, 1fr);
    grid-column-gap: 3px;
    grid-template-rows: repeat(7, 1fr);
    grid-template-areas:
    ". pm pm pm pm pm cs cs cs"
        ". . . . . . . . ."
    ". wr wr wr box1 m1 . ar1 ."
    ". br br br box2 m2 . ar2 ."
      ". . bt bt bt bt bt . ."
      ". . bt bt bt bt bt . ."
        ". . . . . . . . ."
  }
  .pre-made-split {
    grid-area: pm;
    margin-top: .5em;
  }
  .custom-split {
    grid-area: cs;
    margin-top: .5em;
  }
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
