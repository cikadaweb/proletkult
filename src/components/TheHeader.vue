<template>
  <header class="header">
    <nav class="header__nav-list">
      <RouterLink class="header__link link" to="/">Home</RouterLink>
      <RouterLink class="header__link link" :to="{ name: '/projects/[id]', params: { id: 1 } }"
        >Go to Project 1</RouterLink
      >
    </nav>
    <button class="button" type="button">Click me</button>
  </header>
</template>

<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>

<style lang="scss" scoped>
.header {
  padding: 40px;
}
.header__nav-list {
  display: flex;
  gap: 20px;
}
.header__link {
}
</style>
