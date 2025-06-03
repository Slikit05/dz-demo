<script setup>
const date = new Date();
const dateMonth = date.toLocaleDateString()
</script>

<template>
  <div>{{ dateMonth }}</div>
</template>

<style scoped>
</style>