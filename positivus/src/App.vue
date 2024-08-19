<template>
  <HeaderComp msg="Welcome to Your Vue.js App"/>
  <StartInfo />
  <ServicesBlockComp />
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import StartInfo from './components/StartInfo.vue'
import ServicesBlockComp from './components/ServicesBlockComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    StartInfo,
    ServicesBlockComp
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
  padding-left: calc(50% - 620px);
  padding-right: calc(50% - 620px);
}
</style>
