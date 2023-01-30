<template>
  <!-- <PrimeiroComponente/>
  <p>{{ test }}</p>
  <LyfeCycle/> -->
  <Form/>
  <!-- <AtributoDinamico/>
  <Metodos/> -->
  <VFor/>
  <Eventos/>
  <!-- <h1>isso é um props:</h1>
  <Props buttonName="azul"/>
  <Props buttonName="branco"/>
  <Props buttonName="vermelho"/>
  <Props buttonName="amarelo"/>
  <Props buttonName="verde"/> -->
    <h1>Isso é um Emit</h1>
    <Emit/>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponent.vue';
import LyfeCycle from './components/LyfeCycle.vue';
import Form from './components/Form.vue';
import AtributoDinamico from './components/AtributoDinamico.vue';
import Metodos from './components/Metodos.vue';
import VFor from './components/VFor.vue';
import Eventos from './components/Eventos.vue';
import Props from './components/Props.vue';
import Emit from './components/Emit.vue';

export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      LyfeCycle,
      Form,
      AtributoDinamico,
      Metodos,
      VFor,
      Eventos,
      Props,
      Emit,
    },
    data(){
      return{
        test: 'oioi'
      }
    }
  }
</script>

<style>
  body {
    background-color: #333;
    color: #fff;
  }
</style>