<template>
    <h1>atributos dinamicos</h1>
    <p>essee é o <a v-bind:href="linkDinamico" target="blank_" >link</a></p>
    <img :src="avatarDinamico" :alt="descricaoDinamico" >
</template>
<script>
    export default {
        name:'AtributoDinamico',
        data() {
            return {
                linkDinamico: 'https://google.com',
                avatarDinamico: "/img/avatar2.png",
                descricaoDinamico: 'imagem',
            }
        },
    }
</script>