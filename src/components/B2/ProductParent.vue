<template>
  <div>
    <ProductChildren :product="product"></ProductChildren>
  </div>
</template>

<script setup>
import { reactive } from "vue";
import ProductChildren from "./ProductChildren.vue";

const product = reactive({
  id: 1,
  name: "Product 1",
  price: 120000,
  quantity: 10,
});
</script>

<style></style>
