<template>
    <div id="cliente">
        <h4>Nome: {{ nome }}</h4>
        <hr>
        <p>{{ descricao }}</p>
        <hr>
        <p>Número: {{ numero }}</p>
        <p>E-mail: {{ email }}</p>
        <p>Idade: {{ idade }}</p>
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
        nome: String,
        numero: String,
        email: String,
        idade: Number,
        descricao: String,
    }
}
</script>

<style scoped>
    #cliente {
        background-color: #ece5e3;
        font-family: sans-serif;
        max-width: 600px;
        padding: 0.5%;
        margin-top: 2%;
        /*height: 120px;*/
    }
</style>