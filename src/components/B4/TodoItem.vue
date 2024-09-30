<template>
  <div>
    <h2>TodoItem Component</h2>
    <button @click="handleDelete">Delete</button>
  </div>
</template>

<script setup>
import { ref } from "vue";

const id = ref(1);
const emit = defineEmits("delete");
const handleDelete = () => {
  emit("delete", id);
};
</script>

<style></style>
