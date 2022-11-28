<template>
    <Header>
      <img src="../assets/logo.png" alt="">
    </Header>
  </template>
  
  <script>
  export default {
      name:'HeaderComponent',
  }
  </script>
  
  <style lang="scss" scoped>
  *{
      margin: 0 auto;
  }
  header {
      height: 50px;
      background-color: hsl(210deg 21% 23%);
  }
  img {
      height: 50%;      
      padding: 1% 2%;
  }
  </style>