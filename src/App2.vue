<script setup>
    const name="Profesor Nicolás Cáceres Latorre"
    const styleColor = "color:blue"
    const arrayColores = ["blue","red","white"]
    const activo = true
    const arrayFrutas = ["manzana","platano","sandia","frutilla","guinda"]
</script>

<template>
  <h1>Hola {{ name.toUpperCase()  }}</h1>
  <h2 :style = "`color:${arrayColores[2]}`">Soy azul</h2>
  <h2>{{arrayColores}}</h2>
  <p v-if="activo === true">Estoy activo</p>
  <p v-else-if="activo === false">Estoy inactivo</p>
  <p v-else>Estoy indeciso</p>
</template>

<style>
  h1{
    color:red;
  }
</style>