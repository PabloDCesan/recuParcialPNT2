<template>
    <div class="form-group mb-3">
      <label for="input">Ingrese Temperatura °C:</label>
      <input
        id="input"
        type="text"
        class="form-control"
        :value="modelValue"
        @input="$emit('update:modelValue', Number($event.target.value))"
      />
    </div>
  </template>
  
  <script>
  export default {
    props: {
      modelValue: {
        type: Number,
        required: true
      }
    }
  }
  </script>
  