<template>
  <div id="app">
    <h1>Guia Clientes</h1>

    <Cliente
        :cliente="clienteNycolas"
    />

    <Cliente
        :cliente="clienteNycolas"
    />
    
    <Cliente
        :cliente="clienteNycolas"
    />

    
  </div>
</template>

<script>
import Cliente from './components/Cliente.vue';

export default {
  components: { Cliente },
  name: "App",

  data() {
    return {
      clienteNycolas: {
        nome: "Nycolas R. Alves",
        numero: "(83)99960-0613",
        email: "nycolas@gmail.com",
        idade: "19",
        descricao: "Loren ipsum Loren ipsum"
      }
    }
  }
};

</script>

<style>
  #app {
    font-family: sans-serif;
  }
</style>
