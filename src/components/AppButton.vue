<template>
  <div class="app-button">
    <div class="wrapper">
      <div class="text">{{ title }}</div>
      <div class="action">→</div>
    </div>
  </div>
</template>


<script setup>
import { defineProps } from 'vue'
  defineProps(['title']);
</script>

<style lang="scss" scoped>
.app-button {
  width: fit-content;
  transition: all .3s;
  &:hover {
    cursor: pointer;
    border-color: #333;
    background-color: #333;
    color: #fffef2;
  }
  .wrapper {
    display: flex;
    padding: 20px 20px;
    border: solid 1px rgba(51,51,51,.2);
    .action {
      margin-left: 150px;
    }
  }
}
</style>