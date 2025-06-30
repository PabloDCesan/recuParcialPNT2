<template>
  <div class="container">
    <h1>Conversor de temperatura</h1>
    <hr class="separador" />



    <InputTemperatura v-model="celsius" />
    <OutputTemperatura :celsius="celsius" />
  </div>
</template>

<script>
import InputTemperatura from './components/InputTemperatura.vue'
import OutputTemperatura from './components/OutputTemperatura.vue'

export default {
  components: {
    InputTemperatura,
    OutputTemperatura
  },
  data() {
    return {
      celsius: 0
    }
  }
}
</script>

<style>
body {
  font-family: 'Times New Roman', Times, serif;
  background-color: rgb(173, 171, 171);
  color: black;
}
.container {
  max-width: 600px;
  margin: auto;
}

.separador {
  margin-top: 1em;
  margin-bottom: 1em;
}

</style>
