<template>
    <div id="cliente">
        <h4>Nome: {{ cliente.nome }}</h4>
        <hr>
        <p>{{ cliente.descricao }}</p>
        <hr>
        <p>Número: {{ cliente.numero }}</p>
        <p>E-mail: {{ cliente.email }}</p>
        <p>Idade: {{ cliente.idade }}</p>
    </div>
</template>

<script>
export default {
    /*data() {
        return {
            nome: "Nycolas R. Alves",
            numero: "(83)99960-0613",
            email: "nycolasramon3@gmail.com",
            idade: 19,
            descricao: "blablablablabla"
        }
    }*/

    props: {
        cliente: Object,
    }
}
</script>

<style scoped>
    #cliente {
        background-color: #ececec;
        font-family: sans-serif;
        max-width: 600px;
        padding: 0.5%;
        margin-top: 2%;
        /*height: 120px;*/
    }
</style>