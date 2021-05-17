<template>
    <div id="cliente">
        <hr>
        <h4>Nome: {{ cliente.nome }}</h4>
        <hr>
        <p>Número: {{ cliente.numero }}</p>
        <p>E-mail: {{ cliente.email }}</p>

        <!-- Diretiva do Vue.js para condicionar a exibição de um elemento HTML
        O v-else deve ser usado logo abaixo do v-if-->
        <p v-if="showAge">
            Idade: {{ cliente.idade }}
        </p>
        <p v-else>
            O cliente escondeu a idade!
        </p>

        <p v-if="cliente.idade < 18">
            Este cliente é menor de idade!
        </p>
        
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
        showAge: Boolean
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