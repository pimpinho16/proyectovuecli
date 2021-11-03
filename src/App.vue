<template>
  <div >
    <ComponenteSlot>
      hola desde el slot
      <template slot="slot2">

      </template>
    </ComponenteSlot>
  <Usuarios 
    v-for="usuario in usuarios"
    v-bind:key ="usuario.id"
    :nombre = "usuario.name"  
    :email = "usuario.email"
    :telefono = "usuario.phone">
    </Usuarios>
<Padre></Padre>
  </div>
</template>

<script>
import axios from 'axios'
import Usuarios from './components/Usuarios.vue'
import ComponenteSlot from './components/ComponenteSlot.vue'
import Padre from './components/Padre.vue'

  export default {
    name: 'App',
    components: {
      Usuarios,
      ComponenteSlot,
      Padre
    },
    data(){
      return {
        usuarios: [],
      }
    },
    methods:{
      obtenerUsuarios(){
        axios.get('https://jsonplaceholder.typicode.com/users')
        .then((respuesta)=> this.usuarios= respuesta.data)
      }
    },
    mounted(){
      this.obtenerUsuarios()
    }
  }
</script>

<style>

</style>
