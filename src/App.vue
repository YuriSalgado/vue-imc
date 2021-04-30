<template>
  <div id="app">
    <IMC title="Calcule seu IMC" description="Workshop Vue 3"/>
  </div>
</template>

<script>
import IMC from './components/IMC.vue'

export default {
  name: 'App',
  components: {
    IMC
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Roboto+Condensed');

#app {
  font-family: 'Roboto', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
