<template>
  <div id="app">
    <h2>Work in progress...</h2>
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <EllipseComponent/>
  </div>
</template>

<script>
import EllipseComponent from './components/ellipse.vue'

export default {
  name: 'App',
  components: {
    EllipseComponent
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
