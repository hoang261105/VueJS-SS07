<template>
  <button :type="type" @click="handleClick">
    <slot></slot>
  </button>
</template>

<script setup>
const props = defineProps({
  type: {
    type: String,
    default: "button",
  },
});

const emit = defineEmits(["click"]); // Phát sự kiện 'click'

const handleClick = (event) => {
  emit("click", event); // Phát sự kiện click khi button được nhấn
};
</script>

<style>
button {
  /* Ví dụ về style */
  padding: 10px 20px;
  background-color: #007bff;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}
</style>
