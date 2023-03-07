<template>
  <div class="Parcourir">
      <RouterLink v-for="(product, index) in products" :key="index" :to="`/product/${product.id}`">
          <Productcard  :img="product.image" >
         <template #title>{{ product.title }}</template>
         <template #price>{{ product.price }} euros</template>
      </Productcard>


      </RouterLink>
    
     
      
    
   
  </div>
  
</template>

<script setup>
import Productcard from '../components/Productcard.vue';
import { onMounted, ref } from "vue";

const products = ref ([]);

fetch('https://fakestoreapi.com/products')
  .then((response) => response.json())
  .then((data) => {
     
      products.value = data})


</script>

<style scoped>
.Parcourir{
  width: 100%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;

 
  
  
}
</style>