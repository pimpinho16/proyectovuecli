<template>
    <div>
        <p>El nombre es: {{nombre}}</p>
        <p>La edad que tienes es: {{edad}}</p>
    </div>
</template>

<script>
    export default{
        name: "Hijo",
        props:['nombre','edad']
    }
</script>

<style scoped></style>