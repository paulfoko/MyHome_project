<template>
    <img :src="product.image" alt="">
<h3>{{ product.title }}</h3>
<p>{{ product.description }}</p>
<p>{{ product.price }} euros</p>
</template>

<script setup>
import { useRoute } from "vue-router";
import { ref } from "vue";
const route = useRoute()
const product = ref();


fetch(`https://fakestoreapi.com/products/${route.params.id}`)
    .then((response) => response.json())
    .then((data) => {
       
        product.value = data})

</script>

<style>
</style>