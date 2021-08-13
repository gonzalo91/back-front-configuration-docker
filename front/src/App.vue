<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <p>Esooo Estasmos en {{ env }}</p>
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data: () =>{
    return {
      env: process.env.NODE_ENV
    }
  },
  components: {
    HelloWorld
  },
  mounted(){
      console.log(process.env)
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
