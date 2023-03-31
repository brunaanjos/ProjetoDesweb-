<script setup>
import { ref } from 'vue';
const nome = ''
const Email = ''
const Senha = ''
const Confirmar = ''
const moth = ''
const endereco = ''
const cidade = ''
const estado = ''

</script>

<template>
  <h1>Perfil Do Usuario</h1>
  <div>
    <p>Nome</p>
  <input type="text" v-model="nome" 
  placeholder="nome" required/>
  </div>
  
  <div>
    <p>Email</p>
    <input type="email" v-model="Email" 
    placeholder="Email" required/>
  </div>
  <div>
    <p>Senha</p>
<input type="Senha" v-model="Senha" 
placeholder="Senha" required>
</div>
<input type="Confirmar" v-model="Confirmar" 
    placeholder="Confirmar" required/>
<div>
  
  <div class="col-md-3">
    <p>Nacimento</p>
    <label for="validationDefault04" class="form-label"></label>
    <select class="form-select" id="validationDefault04" required>
      <option selected disabled value="">Dia</option>
      <option value="1">1</option>
      <option value="2">2</option>
      <option value="3">3</option>
      <option value="4">4</option>
      <option value="5">5</option>
      <option value="6">6</option>
      <option value="7">7</option>
      <option value="8">8</option>
      <option value="9">9</option>
      <option value="10">10</option>
      <option value="11">11</option>
      <option value="12">12</option>
      <option value="13">13</option>
      <option value="14">14</option>
      <option value="15">15</option>
      <option value="16">16</option>
      <option value="1">17</option>
      <option value="18">18</option>
      <option value="19">19</option>
      <option value="20">20</option>
      <option value="21">21</option>
      <option value="22">22</option>
      <option value="23">23</option>
      <option value="24">24</option>
      <option value="25">25</option>
      <option value="26">26</option>
      <option value="27">27</option>
      <option value="28">28</option>
      <option value="29">29</option>
      <option value="30">30</option>
      <option value="31">31</option>
      
    </select>
    <input type="moth" v-model="Moth">
  </div>
  <div>
    <p>Endereço</p>
    <input type="endereco" v-model="endereco" 
    placeholder="Endereço" required/>
  </div>
  <div>
    <p>Estado</p>
    <input type="estado" v-model="estado" 
    placeholder="Estado" required/>
  </div>
  <div class="col-md-3">
    <p>Estado</p>
    <label for="validationDefault04" class="form-label"></label>
    <select class="form-select" id="validationDefault04" required>
      <option selected disabled value="">Estado</option>
      <option value="">AC</option>
      <option value="2">AL</option>
      <option value="3">AP</option>
      <option value="4">AM</option>
      <option value="5">BA</option>
      <option value="6">CE</option>
      <option value="7">DF</option>
      <option value="8">ES</option>
      <option value="9">GO</option>
      <option value="10">MA</option>
      <option value="11">MT</option>
      <option value="12">MS</option>
      <option value="13">MG</option>
      <option value="14">PA</option>
      <option value="15">PB</option>
      <option value="16">PR</option>
      <option value="1">PE</option>
      <option value="18">PI</option>
      <option value="19">RJ</option>
      <option value="20">RN</option>
      <option value="21">RS</option>
      <option value="22">RO</option>
      <option value="23">RR</option>
      <option value="24">SC</option>
      <option value="25">SP</option>
      <option value="26">SE</option>
      <option value="27">TO</option>
      
    </select>
   
  </div>
</div>

</template>

<style scoped>

</style>
