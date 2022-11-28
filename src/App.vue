<template>
  <div id="app">
    <HeaderComp/>
    <MainComp/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp
  }
}
</script>

<style lang="scss">
  #app {
    font-family: sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    height: 100vh;
    width: 100%;
    background-color: #1E2D3B;
  }
  *{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  .bg-element{
    background-color: #2E3A46;
  }
</style>