<template>
    <h1>EVENTOS</h1>
    <form @submit="enviarFormulario($event)">
        <div>
            <input type="text">
        </div>
        <div>
            <input type="text">
        </div>
        <button @click="mensagem1">Evento @click</button>
    </form>
</template>
<script>
    export default {
        name:'Eventos',
        data() {
            return {

            }
        },
        methods: {
            mensagem1() {
                console.log('botão pressionado 1');
            },
            enviarFormulario(e) {
                e.preventDefault(); //previne de recarregar a pagina
                console.log('formulario enviado');

            }
        }
    }
</script>