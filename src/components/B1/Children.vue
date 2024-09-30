<template>
  <div>
    <h2>Children Component</h2>
    <p>Children Company: {{ props.propName }}</p>
  </div>
</template>

<script setup>
const props = defineProps(["propName"]);
</script>

<style></style>
