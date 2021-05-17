<template>
  <div id="app">
    <h1>Guia Clientes</h1>
    <input type="text" v-model="nomeCliente1">

    <Cliente
        :nome="nomeCliente1"
        numero="(83)99960-0613"
        email="nycolasramon3@gmail.com"
        idade="19"
        descricao="Loren ipsum Loren ipsum"
    />

    <Cliente
        nome="Vitória Ramalho"
        numero="(83)99658-0665"
        email="vitoriaramalho@gmail.com"
        idade="20"
        descricao="Loren ipsum Loren ipsum"
    />

    <Cliente
        nome="Vinicius Fleumático"
        numero="(83)99960-1441"
        email="vinicius@gmail.com"
        idade="22"
        descricao="Loren ipsum Loren ipsum"
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
      nomeCliente1: "Nycolas"
    }
  }
};

</script>

<style>
  #app {
    font-family: sans-serif;
  }
</style>
