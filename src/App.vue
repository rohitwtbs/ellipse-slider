<template>
  <div id="app">
    <p>Work in progress...</p>
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
p {
  animation-duration: 3s;
  animation-name: slidein;
  font-size: 50px;
  font-style: bold;
}

@keyframes slidein {
  from {
    margin-left: 100%;
    width: 300%; 
  }

  to {
    margin-left: 0%;
    width: 100%;
  }
}
</style>
