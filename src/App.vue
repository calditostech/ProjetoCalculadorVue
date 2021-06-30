<template>
  <div id="app">
      <h2>Calculadora</h2>
      <Calculator />
  </div>
</template>

<script>
import Calculator from "./main/Calculator";

export default {
   components: { Calculator }
}
</script>

<style>
@font-face {
  font-family: "RobotoMono";

}

* {
  font-family: "RobotoMono", monospace;
}

body {
  margin: 0;
  background-color: #00BFFF;
}

#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
}

</style>
