<template>
  <div>
    <BaseInput
      placeholder="Enter your name"
      v-model="inputValue"
      @update="handleChange"
    >
      <template #prepend>
        <span>@</span>
      </template>
    </BaseInput>
    <p>Value: {{ inputValue }}</p>
  </div>
</template>

<script setup>
import { ref } from "vue";
import BaseInput from "./BaseInput.vue";

const inputValue = ref("");
const handleChange = (e) => {
  inputValue.value = e;
};
</script>

<style></style>
