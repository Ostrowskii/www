<template>
    <header>
        <nav id="nav">
            <RouterLink to="/" id="logo-url">
                <img :src="logo" :alt="alt" id="logo" >
            </RouterLink>
            <RouterLink to="/">Home</RouterLink>
            <RouterLink to="/pedidos">Pedidos</RouterLink>
        </nav>
    </header>
</template>
<script>
export default{
    name:'Navbar',
    props: ["logo", "alt"],
    data(){

    },
}
</script>
<style scoped>
    #nav{
        background-color: #222;
        border-bottom: 4px solid #111;
        padding: 15px 50px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
        width: 100%;
    }
    #logo-url {
        margin: auto;
        margin-left: 0 !important;
    }
    #logo{
        width: 40px;
        height: 40px;
    }
    #nav a {
        color: #FCBA03;
        text-decoration: none;
        /* margin: 12px; */
        transition: .5s;
    }
    #nav a:not(:first-child) {
        margin: 12px;
    }

    #nav a:hover{
        color: #fff;
    }
</style>