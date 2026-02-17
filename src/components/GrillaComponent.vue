<template>
    <div class="grilla">
        <CardComponent v-for="product in products" :key="product.id" :product="product" />
    </div>
</template>

<script setup>
import CardComponent from './CardComponent.vue';
import { defineProps } from 'vue';

defineProps({
    products: {
        type: Array,
        required: true
    }

})
</script>

<style scoped>
.grilla {
    padding: 15px 20px;
    display: flex;
    flex: row;
    justify-content: space-between;
    flex-wrap: wrap;
}
</style>