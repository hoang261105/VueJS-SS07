<template>
  <div v-if="isClose">
    <h2><slot name="header"></slot></h2>
    <p><slot name="body"></slot></p>
    <button @click="handleClose">Đóng</button>
  </div>
</template>

<script setup>
import { ref } from "vue";

const isClose = ref(true);

const handleClose = () => {
  isClose.value = false;
};
</script>

<style></style>
