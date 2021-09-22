<template>
    <div>
        <p>Nombre: {{nombre}}</p>
        <p>Email: {{email}}</p>
        <p>Telefono: {{telefono}}</p>
        <hr/>
    </div>
</template>

<script>
    export default{
        name: "Usuarios",
       
        props: {
            nombre:String,
            email:String,
            telefono:String
        }
    }
</script>

<style scoped></style>