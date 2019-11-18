<template>
  <div id="app">
    <h1 class="text-center">Conversor de Moedas</h1>
    <div class="linha">
      <Conversor moeda="Dólar americano para real" moedaA="USD" moedaB="BRL"/>
      <Conversor moeda="Real para dólar americano" moedaA="BRL" moedaB="USD"/>
    </div>
    <div class="linha">
      <Conversor moeda="Dólar canadense para real" moedaA="CAD" moedaB="BRL"/>
      <Conversor moeda="Real para dólar canadense" moedaA="BRL" moedaB="CAD"/>
    </div>
    <div class="linha">
      <Conversor moeda="Euro para real" moedaA="EUR" moedaB="BRL"/>
      <Conversor moeda="Real para euro" moedaA="BRL" moedaB="EUR"/>
    </div>
  </div>
</template>

<script>
import Conversor from './components/Conversor.vue'

export default {
  name: 'app',
  components: {
    Conversor
  }
}
</script>

<style>
#app {
  margin: auto;
  max-width: 900px;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
.linha{
  margin-top: 40px;
  display: flex;
  justify-content: space-around;
}
.text-center{
  text-align: center;
}
</style>
