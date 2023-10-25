<template center>
  <h1>
    hi {{name.toUpperCase()}}
  </h1>
  <h2 v-bind:style="styleColor">
    sadasfdasda
  </h2>
  <h3>
    {{ arrayColors }}
  </h3>
  <h4>
    {{ activo ? "estoy activo" : "estoy inactivo"  }}
  </h4>
</template>

<style>
  h1 {
    background-color: green;
    color: white;
    font-family: 'Times New Roman', Times, serif;
  }
  body {
    margin: 0px;
    max-height: 100%;
    max-width: 100%;
  }
  div {
    height: auto;
    width: auto;
  }
</style>

<script setup>
  const name = "vue";
  const styleColor = "color: red";
  const arrayColors = ["blue", "red", "green"];
  const activo = false;
</script>