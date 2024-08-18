<template>
  <div>
    <div class="bg-white shadow-sm p-4">
      <p>{{ product.title }}</p>
      <p>{{ product.price }}</p>
      <p>{{ product.description }}</p>
    </div>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
definePageMeta({
  layout: "products",
});
const uri = `https://fakestoreapi.com/products/${id}`;

// fetch the product
const { data: product } = await useFetch(uri, { key: id });
console.log(product);
</script>

<style scoped></style>
