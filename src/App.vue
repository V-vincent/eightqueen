<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <eight-queen />
  </div>
</template>

<script>
import EightQueen from './components/EightQueen'

export default {
  name: 'App',
  components: {
    EightQueen
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
