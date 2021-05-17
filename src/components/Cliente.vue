<template>
    <div id="cliente">
        <hr>
        <h4>Nome: {{ cliente.nome }}</h4>
        <hr>
        <p>Número: {{ cliente.numero }}</p>
        <p>E-mail: {{ cliente.email }}</p>

        <!-- Diretiva do Vue.js para exibir um elemento HTML
        caso showAge for verdadeira
        
        O resultado é o mesmo do v-if, só que tem 2 diferenças:
            - Mesmo com o v-show falso, o Vue não deleta o elemento;
            - Não existe else para v-show.
        -->
        <p v-show="showAge">
            Idade: {{ cliente.idade }}
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