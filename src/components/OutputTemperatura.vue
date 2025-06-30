<template>
    <div>
      <label>Conv Temperatura °F: <span style="color: blue">{{ fahrenheit.toFixed(2) }} °F</span></label>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      celsius: {
        type: Number,
        required: true
      }
    },
    computed: {
      fahrenheit() {
        return (this.celsius * 9) / 5 + 32
      }
    }
  }
  </script>
