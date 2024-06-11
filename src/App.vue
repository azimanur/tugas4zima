<template>


    <div id="app">
      <Emit />
    </div>
  </template>
  
  <script>
  import Emit from './components/Emit.vue';
  
  export default {
    components: {
      Emit,
    },
  };
  </script>
  
  <style scoped>
  #app {
    font-family: Avenir, Helvetica;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: rgba(245, 245, 245, 0.758);
  }
  </style>