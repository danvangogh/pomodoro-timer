<template>
  <div id="app">
    <Header />
    <Description />
    <ClockSelection />
    <Timer />
    <Hourglass />
  </div>
</template>

<script>
import Header from './components/Header';
import Description from './components/Description';
import ClockSelection from './components/ClockSelection';
import Timer from './components/Timer';
import Hourglass from './components/Hourglass';

export default {
  name: 'App',
  components: {
    Header,
    Description,
    ClockSelection,
    Timer,
    Hourglass,
  },
}
</script>

<style>

  body {
    margin: 0;
    padding: 0;
    background-color: #242424;
  }

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #E6E6E6;
  height: 100vh;
  display: grid;
  grid-template-columns: 1fr 400px 1fr 400px 1fr;
  grid-template-areas:
  "h h . . ."
  ". d . tm ."
  ". cs . hg ."
  ;
  grid-template-rows: 75px 1fr 1fr;
}
p {
  font-size: 12px
}
</style>
