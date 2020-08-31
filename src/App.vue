<template>
  <div>
    <encabezado />
    <contenido />
    <pieDepagina/>
    </div>
</template>

<script>
 import encabezado from "./components/encabezado"
 import contenido from "./components/contenido"
 import pieDepagina from "./components/pieDepagina"

 export default {
   name: "App",
   components: {
     encabezado,
     contenido,
     pieDepagina
   }
 };
</script>

<style>

</style>