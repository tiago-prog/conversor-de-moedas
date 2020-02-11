<template>
  <div id="app">
    <h1 class="text-center">Conversor de Moedas</h1>
    <div class="linha">
      <Conversion moedaA="USD" moedaB="BRL"/>
      <Conversion moedaA="BRL" moedaB="USD"/>
    </div>
    <div class="linha">
      <Conversion moedaA="CAD" moedaB="BRL"/>
      <Conversion moedaA="BRL" moedaB="CAD"/>
   </div>
  <div class="linha">
    <Conversion moedaA="EUR" moedaB="BRL"/>
    <Conversion moedaA="BRL" moedaB="EUR"/>
  </div>
  </div>
</template>

<script>
import Conversion from './components/Conversion.vue'

export default {
  name: 'App',
  components: {
    Conversion
  }
}
</script>

<style>
#app {
  margin: auto;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}

.linha {
  display: flex;
  justify-content: space-around;
  margin-top: 25px;
}

.text-center {
  text-align: center;
}
</style>
