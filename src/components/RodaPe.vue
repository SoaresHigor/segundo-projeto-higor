  <div class="hello">
    
  </div>
  <template>
    <div>
      <strong><p>Responda nossa enquete!</p></strong>
      <button @click="coletarDados">Nome</button>
      <button @click="coletarDados">Email</button>
      <button @click="coletarDados">Teria interesse em visitar nossa cidade?</button>
      <p v-if="dadosArmazenados">Dados Armazenados:</p>
      <ul v-if="dadosArmazenados">
        <li>Nome: {{ dadosArmazenados.nome }}</li>
        <li>Email: {{ dadosArmazenados.email }}</li>
        <li>Interesse: {{ dadosArmazenados.interesse }}</li>
      </ul>
    </div>
    <footer>
      <strong>
      <p>Higor 2024 © TODOS OS DIREITOS RESERVADOS</p>
      </strong>
    </footer>
    
  </template>
  
<script>
export default {
  data() {
    return {
      dadosArmazenados: null
    }
  },
  methods: {
    coletarDados() {
      const nome = prompt("Digite seu nome:");
      const email = prompt("Digite seu email:");
      const interesse = prompt("Sim ou não?")
      if (nome && email) {
        this.dadosArmazenados = {
          nome: nome,
          email: email,
          interesse: interesse
        };
        localStorage.setItem("dados", JSON.stringify(this.dadosArmazenados));
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
  color: rgb(38, 75, 3);
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
button {
  display: table-row;
}
</style>
