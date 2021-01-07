<template>
  <div id="app">
    <!-- <img src="./assets/logo.png">
    <router-view/> -->
    <Vant />
  </div>
</template>

<script>
import Vant from './components/Vant';
export default {
  name: 'App',
  components: {
    Vant
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
