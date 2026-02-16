<template>

<GrillaComponent
:products="products"/>

</template>


<script setup>
import { ref } from 'vue';
import productAll from "./assets/data/products.json"
import GrillaComponent from './components/GrillaComponent.vue';

const products= ref (productAll)
console.log (products.value)

</script>

<style>

</style>
