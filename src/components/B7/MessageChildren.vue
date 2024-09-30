<template>
  <div>
    <button @click="handleClick">Send message</button>
  </div>
</template>

<script setup>
const data = "Rikkei Education";
const emit = defineEmits("alert");
const handleClick = () => {
  emit("alert", data);
};
</script>

<style></style>
