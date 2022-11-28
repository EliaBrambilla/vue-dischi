<template>
    <div class="bg-element">
      <img src="../assets/logo.svg" alt="">
    </div>
  </template>
  
  <script>
  export default {
    name: 'HeaderComp',
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">
    
    div{
      padding: 20px;
      height: 90px;
      display: flex;
      justify-content: flex-start;
      align-items: center;
    }
    img{
      height: 100%;
    }
  </style>