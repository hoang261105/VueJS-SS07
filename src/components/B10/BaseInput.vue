<template>
  <div>
    <input
      :type="type"
      :placeholder="placeholder"
      :value="modelValue"
      @input="handleChange"
    />
  </div>
</template>

<script setup>
const props = defineProps({
  placeholder: {
    type: String,
    default: "",
  },
  type: {
    type: String,
    default: "text", // Giá trị mặc định là 'text'
  },
  modelValue: {
    type: [String, Number],
    default: "", // Giá trị mặc định là chuỗi rỗng
  },
});

const emit = defineEmits("update");
const handleChange = (e) => {
  emit("update", e.target.value);
};
</script>

<style scoped>
.input-container {
  display: flex;
  align-items: center;
}

input {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  flex-grow: 1;
}

input:focus {
  border-color: #007bff;
  outline: none;
}
</style>
