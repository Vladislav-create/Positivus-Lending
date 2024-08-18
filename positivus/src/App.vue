<template>
  <HeaderComp msg="Welcome to Your Vue.js App"/>
  <StartInfo />
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import StartInfo from './components/StartInfo.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    StartInfo
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
