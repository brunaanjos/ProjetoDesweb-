<script setup>
import { ref } from 'vue';
const nome = ''
const Email = ''
</script>

<template>
  <h1>Perfil Do Usuario</h1>
  <div>
  <input type="text" v-model="nome" 
  placeholder="nome" required/>
  </div>
  
  <div>
    <input type="email" v-model="Email" 
    placeholder="Email" required/>
  </div>
  <div>
<input type="Senha" v-model="Senha" placeholder="Senha" required>

  </div>

</template>

<style scoped>

</style>
