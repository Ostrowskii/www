<template>
  <div id="pag">
    <Navbar :logo="logo_src" :alt="app_name" />
    <RouterView />
    <Footer/>
  </div>
</template>


<script>
  import Navbar from "./components/Navbar.vue";
  import Footer from "./components/Footer.vue";
  import { RouterLink, RouterView } from 'vue-router';

  export default{
    components:{
      Navbar,
      Footer,
    },
    data(){
      return{
        logo_src: "/img/logo.png",
        app_name: "Make Your Burg",
      }
    }
  }
</script>


<style>
*{
  font-family: Helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.main-container{
  margin: 50px;
  min-height: 250px;
}
h1{
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
#pag{
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

</style>
