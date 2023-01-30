<template>
    <h1>METODOS</h1>
    <button @click="showEmail" >Mostrar email</button>
    <p v-show="isShowEmail">este é meu email: {{ email }}</p>
</template>
<script>
    export default {
        name: 'Metodos',
        data() {
            return {
                email:'joao@gmail.com',
                isShowEmail: false,
            }
        },
        methods: {
            showEmail(){
                this.isShowEmail = !this.isShowEmail; 
            }
        }
    }
</script>

