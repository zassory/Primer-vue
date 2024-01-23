<script setup>
    const name="Profesor Nicolás Cáceres Latorre"    
    const arrayFrutas = ["manzana","platano","sandia","frutilla","guinda"]
</script>

<template>
  <h1>Hola {{ name  }}</h1>
  <ul>
    <li 
      v-for="(fruta , index) in arrayFrutas"
      :key="index"
      >
      {{index+1}} - {{fruta}}
    </li>
  </ul>
</template>

<style>
  h1{
    color:red;
  }
  ul{
    color: white;
  }
</style>