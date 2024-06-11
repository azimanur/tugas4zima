<template>
    <div class="gtu">
      <h2>Bismillah Yang tekan tombol akan sukses</h2>
      <Enmit2 @message-from-grandchild="ehe" />
      <slot name="additionalContent"></slot>
    </div>
  </template>
  
  <script>
  import Enmit2 from './Emit2.vue';
  
  export default {
    components: {
      Enmit2,
    },
    methods: {
      ehe(payload) {
        this.$emit('message-from-child', payload);
      },
    },
  };
  </script>
  
  <style scoped>
  .Guts {
    padding: 15px;
    background-color: #040404;
    border: 1px solid #2c2121;
    border-radius: 5px;
    margin-top: 10px;
  }
  </style>
  
  