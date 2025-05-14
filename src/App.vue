<script setup>
import Header from './components/Header.vue';
import StatusInicial from './components/Status-inicial.vue';
import Menu1 from './components/Menu-1.vue';
</script>

<template>
  <div class="app-container">
    <Header />
    <StatusInicial />
    <Menu1 />
  </div>
</template>

<style scoped>
.app-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: rgb(235, 235, 235);
}
</style>



