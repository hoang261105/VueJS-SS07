<template>
  <div>
    <h1>Parent Component</h1>
    <p>Parent company: {{ company }}</p>
    <Children :propName="company"></Children>
  </div>
</template>

<script setup>
import Children from "./Children.vue";
const company = "Rikkei Academy";
</script>

<style></style>
