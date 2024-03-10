<script setup>
  import { ref } from "vue"
  const value = ref(0)
</script>

<template>
  <div class="container">
    <div class="header">JavaScript Counter</div>
    <div class="value" id="value">{{ value }}</div>
    <div class="buttons">
      <button @click="value--">-</button>
      <button @click="value++">+</button>
    </div>
  </div>
</template>

<style lang="scss">

  .container {
    background: white;
    padding: 2rem;
    border-radius: 15px;
    .header {
      font-size: 1.7rem;
      color: #7e7c7c;
    }
    .value  {
      display: flex;
      justify-content: center;
      font-size: 5rem;
      color: #8a8a8a;
    }
    .buttons {
      display: flex;
      justify-content: center;
      gap: 5px;
      button {
        padding: 5px 20px;
        font-size: 1.2rem;
        border: none;
        border-radius: 5px;
        display: flex;
        align-items: center;
        justify-content: center;
      }
    }
  }

</style>
