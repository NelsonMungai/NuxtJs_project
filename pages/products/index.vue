<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div
        v-for="(p, index) in products"
        :key="index"
        class="bg-white shadow-sm p-2"
      >
        <NuxtLink :to="`/products/${p.id}`">{{ p.title }}</NuxtLink>
      </div>
      <h1>Products</h1>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: "products",
});
// fetch the data
const {
  data: products,

  error,
} = await useFetch("https://fakestoreapi.com/products");

// Optionally handle the state of your request
</script>

<style scoped></style>
