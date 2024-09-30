<template>
  <div>
    <BaseButton @click="handleSubmit">Submit</BaseButton>
  </div>
</template>

<script setup>
import BaseButton from "./BaseButton.vue";
const handleSubmit = () => {
  console.log("Submit button clicked");
};
</script>

<style></style>
