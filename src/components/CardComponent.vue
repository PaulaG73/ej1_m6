<template>
    <div class="card">
        <div class="container">
            <h4>Nombre:{{ name }}</h4>
            <p>Descripción:{{ description }}</p>
            <p>Precio:{{ precio }}</p>
            <p>Disponible:{{ active }}</p>
        </div>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';
defineProps({
    name:{
        type:String
    },
    description:{
        type:String
    },
    precio:{
        type:Number
    },
    active:{
        type:Boolean
    }

})


</script>

<style>

</style>