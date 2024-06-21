<template>
  <img alt="Vue logo" src="./assets/turismo-Aripuana.webp">
  <CabecalhoCima msg=" "/>
  <menu-meio msg="  "/>
  <HistoriaAripaVue msg="  "/>
  <ConteudoPrincipal msg="  "/>
  <RodaPe msg="  "/>
  </template>
<script>
import CabecalhoCima from './components/CabecalhoCima.vue'
import MenuMeio from './components/MenuMeio.vue'
import HistoriaAripaVue from './components/HistoriaAripa.vue';
import RodaPe from './components/RodaPe.vue';
import ConteudoPrincipal from './components/ConteudoPrincipal.vue';

export default {
  name: 'App',
  components: {
    CabecalhoCima,
    MenuMeio,
    RodaPe,
    HistoriaAripaVue,
    ConteudoPrincipal
   }
}
</script>
<style>
#app {
  background-color:#c2c2c200;
  font-family: Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  width: 1300px;
  padding: 10px;
}

img {
  height: 472px;
  width: 900px;
  padding: 1px;
}
</style>
