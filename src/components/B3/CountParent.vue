<template>
  <div>
    <h2>Parent Component</h2>
    <p>Count: {{ number }}</p>
    <CountChildren @messageSent="handleClick"></CountChildren>
  </div>
</template>

<script setup>
import { ref } from "vue";
const number = ref(0);

import CountChildren from "./CountChildren.vue";
const handleClick = () => {
  number.value++;
};
</script>

<style></style>
