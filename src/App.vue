<script setup>
import Header from './components/Header.vue';
import StatusInicial from './components/Status-inicial.vue';
import Menu1 from './components/Menu-1.vue';
import MenuBottom from './components/Menu-Bottom.vue';
import Conteudo from './components/Conteudo.vue';
</script>

<template>
  <div class="app-container">
    <Header />
    <StatusInicial />
    <Menu1 />
    <MenuBottom />  
    <Conteudo />
  </div>
</template>

<style scoped>
.app-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>



