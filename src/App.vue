<template>
<NavBarComponent/>
<GrillaComponent
:products="products"/>

</template>


<script setup>
import NavBarComponent from './components/NavBarComponent.vue';
import { ref } from 'vue';
import productAll from "./assets/data/products.json"
import GrillaComponent from './components/GrillaComponent.vue';

const products= ref (productAll)
console.log (products.value)

</script>

<style>

</style>
