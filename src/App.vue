<template>
  <div >
    <Persona nombre="Manuel" edad = 27></Persona>
    <hr/>
    <Persona nombre="Alex" edad = 32></Persona>
  </div>
</template>

<script>
  import Persona from "./components/Persona"


  export default {
    name: 'App',
    components: {
      Persona,
    }
  }
</script>

<style>

</style>
