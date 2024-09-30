<template>
  <MessageChildren @alert="handleClick" />
</template>

<script setup>
import MessageChildren from "./MessageChildren.vue";
const handleClick = (data) => {
  alert(`Welcome to ${data}`);
};
</script>

<style></style>
