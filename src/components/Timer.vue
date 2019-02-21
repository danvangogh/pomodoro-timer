<template>
  <div class="timer">
    <div class="card">
      <h5>Time left to Science:</h5>
      <div class="time-display"></div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Timer',
  components: {
  },
  data () {
    return {
      workTime: 0,
      breakTime: 0,
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .timer {
    grid-area: tm;
    padding: 1em;
    color: white;
    margin: auto;
  }
  .card {
    margin: auto;
    width: 280px;
    height: 110px;
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
    grid-template-rows: 1fr 3fr;
    line-height: 0px;
    text-align: center;
  }
  .time-display {
    
  }

</style>
