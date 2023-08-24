<template>
  <div id="app">

    <CabezeraHome :msg="mensaje"/>
    <ListaHome/>

  </div>
</template>

<script>
import CabezeraHome from './components/CabezeraHome.vue';
import ListaHome from './components/ListaHome.vue';

export default {
  name: 'App',
  components: {
    CabezeraHome,
    ListaHome,
  },
  
  data() {
    return {
      mensaje: 'Aplicacion de Vue titulo'
    }
  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
