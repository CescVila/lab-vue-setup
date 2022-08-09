<template>
  
  <NavComponent />
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <FooderComponent />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import NavComponent from './components/NavComponent.vue'
import FooderComponent from './components/FooderComponent.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    NavComponent,
    FooderComponent
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
