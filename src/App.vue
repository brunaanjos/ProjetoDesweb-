<script setup>
import { ref } from 'vue';
const nome = ref('')
const Email = ref('')
const Senha = ref('')
const Confirmar = ref('')
const Month = ref('')
const endereco = ref('')
const estado = ref('')
const Hobbie = ref('')
const Linguagem = ref('')
const Biografia = ref('')
const Mostar = ref(false)

</script>

<template>
  <div id="editor">
    <form @submit.prevent="Mostar = !Mostar">
      <h1>Perfil Do Usuario</h1>
      <div>
        <p>Nome</p>
        <input type="text" v-model="nome" placeholder="nome" required />
      </div>

      <div>
        <p>Email</p>
        <input type="email" v-model="Email" placeholder="Email" required />
      </div>
      <div>
        <p>Senha</p>
        <input type="Senha" v-model="Senha" placeholder="Senha" required>
        
        <div>
          <input type="Confirmar" v-model="Confirmar" placeholder="Confirmar" required />
        </div>
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
          <option value="17">17</option>
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
        <input type="Month" v-model="Month">
      </div>
      <div>
        <p>Endereço</p>
        <input type="endereco" v-model="endereco" placeholder="Endereço" required />
      </div>

      <div>
        <p>Estado</p>
        <label for="validationDefault04" class="form-label"></label>
        <select class="form-select" id="validationDefault04" required>
          <option selected disabled value="">Estado</option>
          <option value="Acre">AC</option>
          <option value="Alagoas">AL</option>
          <option value="Amapá">AP</option>
          <option value="Amazonas">AM</option>
          <option value="Bahia">BA</option>
          <option value="Ceará">CE</option>
          <option value="Distrito Federal">DF</option>
          <option value="Espírito Santo">ES</option>
          <option value="Goiás">GO</option>
          <option value="Maranhão">MA</option>
          <option value="Mato Grosso">MT</option>
          <option value="Mato Grosso do Sul">MS</option>
          <option value="Minas Gerais">MG</option>
          <option value="Pará">PA</option>
          <option value="Paraíba">PB</option>
          <option value="Paraná">PR</option>
          <option value="Pernambuco">PE</option>
          <option value="Piauí">PI</option>
          <option value="Rio de Janeiro">RJ</option>
          <option value="Rio Grande do Norte">RN</option>
          <option value="Rio Grande do sul">RS</option>
          <option value="Rondônia">RO</option>
          <option value="Roraima">RR</option>
          <option value="Santa Catarina">SC</option>
          <option value="São Paulo">SP</option>
          <option value="Sergipe">SE</option>
          <option value="Tocantis">TO</option>

        </select>

      </div>
      <div>
        <p>Hobbies</p>
        <input type="text" v-model="Hobbie" placeholder="Diga o seu Hobbie" required />
      </div>
      <div>
        <p>Linguagem</p>
        <label for="validationDefault04" class="form-label"></label>
        <select class="form-select" aria-label="Default select exemple" required>
          <option selected disabled value="">Linguagem</option>
          <option value="Python">Python</option>
          <option value="PHP">PHP</option>
          <option value="JavaScript">JavaScript</option>
          <option value="Swift">Swift</option>
          <option value="Java">Java</option>
          <option value="Go">Go</option>
          <option value="SQL">SQL</option>
          <option value="Ruby">Ruby</option>

        </select>

      </div>

      <p>Biografia</p>
      <textarea class="form-control" id="validationTextarea" placeholder="Required example textarea" required></textarea>
      <div>
        <p> </p>
        <button type="button" class="btn btn-outline-light">Enviar</button>
      </div>

      <div v-if="Mostar">

        <div>Nome:{{ nome }}</div>
        <div>Email:{{ Email }}</div>
        <div>Senha:{{ Senha }}</div>
        <div>Confirmar:{{ Confirmar }}</div>
        <div>Data Nascimento:{{ Month }}</div>
        <div>Endereço:{{ endereco }}</div>
        <div>estado:{{ estado }}</div>
        <div>Hobbie:{{ Hobbie }}</div>
        <div>Biografia:{{ Biografia }}</div>
        <div>Linguagem:{{ Linguagem }}</div>

      </div>
    </form>
  </div>
</template>

<style scoped>
#editor {
  text-align: center;
  margin: 5px;
  background-color: rgb(195, 142, 231);
  border-radius: 6px;
  border-color: rgb(40, 172, 212);
  border-style: unset;
  color: rgb(255, 255, 255);
  padding: 15px

}
</style>
