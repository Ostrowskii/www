<template>
    <img :src=avatar>
    <ChangeImage @mudar-imagem="trocarImagem" />
</template>
<script>

    import ChangeImage from './emit/ChangeImage.vue';

    export default{
        name:'Emit',
        components: {
            ChangeImage,
        },
        data() {
            return {
                avatar: '../../public/img/avatar1.jpg',
            }
        },
        methods: {
            trocarImagem() {
                console.log("opa");
                this.avatar = "../../public/img/avatar2.png";
            }
        }
        
    }
</script>
<style>
    img{
        height: 100px;
    }
</style>