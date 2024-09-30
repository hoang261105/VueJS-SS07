<template>
  <div>
    <h2>Children Component</h2>
    <button @click="handleClick">Increase</button>
  </div>
</template>

<script setup>
const emit = defineEmits("messageSent");
const handleClick = () => {
  emit("messageSent");
};
</script>

<style></style>
