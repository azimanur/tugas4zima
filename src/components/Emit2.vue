
<template>
    <div class="container">
      <button @click="goEmit">Tekan disini</button>
    </div>
  </template>
  
  <script>
export default {
  methods: {
    goEmit() {
      alert("Amin Yallah Semoga terkabulkan");
    },
  },
};
  </script>
  
  <style scoped>
  
  button {
    padding: 1rem 2rem;
    border: none;
    border-radius: 16px;
    background-color: #ead3fa;
    color: rgb(29, 28, 31);
    cursor: pointer;

  }
  button:hover {
    background-color: #e8ecf9;
    transition: 0.5ms;
  }
  </style>
  
