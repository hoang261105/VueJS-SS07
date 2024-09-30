<template>
  <div>
    <h2>Dữ liệu trong component con</h2>
    <p>Id: {{ productDetail.product.id }}</p>
    <p>Product: {{ productDetail.product.name }}</p>
    <p>Price: {{ productDetail.product.price }}</p>
    <p>Quantity: {{ productDetail.product.quantity }}</p>
  </div>
</template>

<script setup>
const productDetail = defineProps(["product"]);
</script>

<style></style>
