<script setup>
import Titulo from './components/Titulo.vue'
import ListaNomes from './components/ListaNomes.vue';
import Cartao from './components/Cartao.vue';
</script>

<template>

  <div>
    <Titulo />
    <ListaNomes />
    <Cartao 
      nome="Gilberto"
      curso="Agronomia"
    />

  </div>
  
</template>

<style scoped></style>
