<template>
    <div id="cliente">
        <!-- Para se obter o valor de uma variável em um atributo, usa-se o ":"
        Isto é fazer um data binding, ou seja, se está ligando um campo de um formulário
        
        Isso é um one way data binding: para leitura -->
        <input type="text" :value="nome">
        <hr>
        <input type="text" :value="descricao">
        <hr>

        <!--Two way data binding: para leitura e edição-->
        <input type="text" v-model="email">
        <hr>

        <!-- Os valores das variáveis são recuperados do objeto
        retornado pela função data() -->
        <h2 id="cliente-nome">Dados do cliente: {{ nome }}</h2>
        <p>Descrição do cliente: {{ descricao }}</p>
        <p>Email do cliente: {{ email }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            nome: "Nycolas R. Alves",
            numero: "(83)99960-0613",
            email: "nycolasramon3@gmail.com",
            idade: 19,
            descricao: "Descrição do cliente Nycolas"
        }
    }
}
</script>

<style scoped>
    #cliente {
        max-width: 600px;
        height: 120px;
    }
</style>