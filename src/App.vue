<script setup>
import { ref } from 'vue';
const nome = ref('')
const email = ref('')
const senha = ref('')
const month = ref('')
const endereco = ref('')
const estado = ref('')
const hobbie = ref('')
const linguagem = ref('')
const biografia = ref('')

const viewSenha = ref(false)
const viewConfirmarSenha = ref(false)
const mostrar = ref(true)
</script>

<template>
  <div id="editor">

    <form @submit.prevent="mostrar = !mostrar">

      <h1>Cadastrar-se</h1>
      <div>
        Nome:
        <input type="text" v-model="nome" placeholder="nome" required />
      </div>

      <div>
        Email:
        <input type="email" v-model="email" placeholder="email" required />
      </div>
      <div>
        Senha:
        <div class="input-group mb-3">
          <input :type="viewSenha ? 'text' : 'password'" v-model="senha" placeholder="Senha" required>
          <button class="btn" @click="viewSenha = !viewSenha">{{ viewSenha ? 'Mostrar' : 'Ocultar' }}</button>
        </div>
        <div>
          Confirmar:
          <div class="input-group mb-3">
            <input :type="viewConfirmarSenha ? 'text' : 'password'" v-model="viewConfirmarSenha" placeholder="Senha"
              required>
            <button class="btn" @click="viewConfirmarSenha = !viewConfirmarSenha">{{ viewConfirmarSenha ? 'Mostrar' :
              'Ocultar' }}</button>
          </div>
        </div>
        Nascimento:


        <input type="Date" v-model="month">
      </div>
      <div>

        Endereço:
        <input type="endereco" v-model="endereco" placeholder="Endereço" required />
      </div>

      <div>
        Estado:

        <label for="validationDefault04" class="form-label"></label>
        <select class="form-select" v-model="estado" id="validationDefault04" required>
          <option selected disabled value="">estado</option>
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
        <p>hobbies</p>
        <input type="text" v-model="hobbie" placeholder="Diga o seu Hobbie" required />
      </div>
      <div>
        <label for="validationDefault04" class="form-label"></label>
        <select class="form-select" v-model="linguagem" aria-label="Default select exemple" required>
          <option selected disabled value="">linguagem</option>
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

      <p>biografia</p>
      <textarea class="form-control" v-model="biografia" id="validationTextarea" placeholder="Required example textarea"
        required></textarea>
      <div>
        <p> </p>
        <button type="submit" class="btn btn-outline-light">Enviar</button>
      </div>

      <div v-if="mostrar">

        <div>Nome:{{ nome }}</div>
        <div>Email:{{ email }}</div>
        <div>Senha:{{ senha }}</div>
        <div>Confirmar:{{ confirmar }}</div>
        <div>Data Nascimento:{{ month }}</div>
        <div>Endereço:{{ endereco }}</div>
        <div>Estado:{{ estado }}</div>
        <div>Hobbie:{{ hobbie }}</div>
        <div>Biografia:{{ biografia }}</div>
        <div>Linguagem:{{ linguagem }}</div>

      </div>
    </form>
  </div>
</template>

<style scoped>
#editor {
  text-align: left;
  margin-left: 500px;
  margin-right: 500px;
  background-color: rgb(134, 33, 218);
  border-radius: 50px;
  border-style: unset;
  color: rgb(236, 216, 216);
  padding: 70px
}
</style>
