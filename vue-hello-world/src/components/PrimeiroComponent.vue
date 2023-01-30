<template>
    <h1>Olá Vue</h1>
    <p> Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    <form>
        <input type="text" v-model="input_name">
        <input type="submit" value="Enviar" v-on:click="submitForm">
    </form>
    {{ input_name }}
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
        data() {
            return {
                nome:"Matheus",
                profissao: "programador",
                input_name: "",
            }
        },
        methods: {
            submitForm(e){
                e.preventDefault();
                this.nome = this.input_name
                console.log("aqui");
            }
        }
    }
</script>