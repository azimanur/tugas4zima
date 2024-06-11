<template>
    <div class="container">
      <h1>Jadi orang sukses</h1>
      <p>{{ message }}</p>
      <Slot @message-from-child="handleMessageFromChild">
        <template v-slot:additionalContent>
          <p> Ingat!! kesuksesan ada di diri kita sendiri. </p>
          <p>Jangan putus asa dalam menjalani kehidupan ini </p>
        </template>
      </Slot>
    </div>
  </template>
  
  <script>
  import Slot from './Slot.vue';
  
  export default {
    components: {
      Slot,
    },
    data() {
      return {
        message: '',
      };
    },
    methods: {
      handleMessageFromChild(payload) {
        this.message = payload;
      },
    },
  };
  </script>
  
 <style scoped>
.container {
  background-color: rgba(255, 255, 255, 0.08);
  border-radius: 10px;
}
</style>