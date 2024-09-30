<template>
  <div>
    <!-- Bài 1 -->
    <Parent></Parent>
    <br />
    <!-- Bài 2 -->
    <ProductParent></ProductParent>
    <br />
    <!-- Bài 3 -->
    <CountParent></CountParent>
    <br />
    <!-- Bài 4 -->
    <TodoApp></TodoApp>
    <br />
    <!-- Bài 5 -->
    <Modal>
      <template #header>Thông báo từ hệ thống</template>
      <template #body
        >Đây là nội dung của modal. Bạn có thể đóng modal bằng cách nhấn vào nút
        'Close'.</template
      >
    </Modal>
    <br />
    <!-- Bài 6 -->
    <Cart>
      <template #header>Thông tin sản phẩm</template>
      <template #body
        >Đây là mô tả ngắn gọn về sản phẩm này. Sản phẩm có các tính năng nổi
        bật và giá cả hợp lý.</template
      >
      <template #footer>Xem chi tiết</template>
    </Cart>
    <br />
    <!-- Bài 7 -->
    <MessageParent />
    <br />
    <!-- Bài 8 -->
    <ListUser />
    <br />
    <!-- Bài 9 -->
    <Button></Button>
    <br />
    <!-- Bài 10 -->
    <InputValue />
  </div>
</template>

<script setup>
import Parent from "./components/B1/Parent.vue";
import ProductParent from "./components/B2/ProductParent.vue";
import CountParent from "./components/B3/CountParent.vue";
import TodoApp from "./components/B4/TodoApp.vue";
import Modal from "./components/B5/Modal.vue";
import Cart from "./components/B6/Cart.vue";
import MessageParent from "./components/B7/MessageParent.vue";
import ListUser from "./components/B8/ListUser.vue";
import Button from "./components/B9/Button.vue";
import InputValue from "./components/B10/InputValue.vue";
</script>

<style></style>
