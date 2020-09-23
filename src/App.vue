<template>
  <div id="app">
    <h1 class="text-center">Conversor de Moedas</h1>

    <div class="linha">
      <Conversor moeda-a="USD" moeda-b="BRL"></Conversor>
      <Conversor moeda-a="BRL" moeda-b="USD"></Conversor>
    </div>

    <div class="linha">
      <Conversor moeda-a="CAD" moeda-b="BRL"></Conversor>
      <Conversor moeda-a="BRL" moeda-b="CAD"></Conversor>
    </div>

    <div class="linha">
      <Conversor moeda-a="EUR" moeda-b="BRL"></Conversor>
      <Conversor moeda-a="BRL" moeda-b="EUR"></Conversor>
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor";

export default {
  name: 'App',
  components: {
    Conversor
  }
}
</script>

<style>
#app {
  margin: auto;
  max-width: 900px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}

.linha {
  display: flex;
  margin-top: 40px;
  justify-content: space-around;
}

.text-center{
  text-align: center;
}
</style>
