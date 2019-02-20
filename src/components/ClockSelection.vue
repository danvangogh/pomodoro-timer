<template>
  <div class="clock">
    <div class="card">
      <span class="pre-made-split">Pre-made Splits</span>
      <span class="custom-split">Custom</span>
      <PreMadeForm />
    </div>
  </div>
</template>

<script>
  import PreMadeForm from './PreMadeForm'
  import CustomForm from './CustomForm'
export default {
  name: 'ClockSelection',
  components: {
    PreMadeForm,
  },
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
    grid-template-rows: repeat(7, 1fr);
    grid-column-gap: 3px;
  }
  .pre-made-split {
    grid-column: 2/6;
    margin-top: .5em;
  }
  .custom-split {
    grid-column: 7/9;
    margin-top: .5em;
  }
</style>
