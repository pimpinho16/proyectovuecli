<template>
    <div>
         <h1 style="color:red">
             /*solo puede haber un slot */
            <slot>
                hola desde el componente
            </slot>
         </h1>
           <h2 >
             
            <slot name="slot2">
                hola desde el componente 2
            </slot> 
         </h2>
    </div>
</template>

<script>
    export default{
        name: "ComponenteSlot"
    }
</script>

<style scoped></style>