<template>
  <div>
    <h2>TodoApp Component</h2>
    <p>Id to delete: {{ count }}</p>
    <TodoItem @delete="handleDelete"></TodoItem>
  </div>
</template>

<script setup>
import { ref } from "vue";
import TodoItem from "./TodoItem.vue";
let count = ref(0);

const handleDelete = (data) => {
  count.value = data;
};
</script>

<style></style>
