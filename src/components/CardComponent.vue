<template>
    <div class="card">
        <div class="container">
            <h4>Nombre:{{ product.name }}</h4>
            <p>Descripción:{{ product.description }}</p>
            <p>Precio:{{ product.precio }}</p>
            <p>Disponible:{{ product.active }}</p>
        </div>
    </div>

  
</template>

<script setup>

import { defineProps } from 'vue';
defineProps({
    product:{
        type: Object,
        required: true
    }

})


</script>

<style>




</style>