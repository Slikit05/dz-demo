<script setup>
import Heart from '../icons/Heart.vue';

const { label } = defineProps({
  label: String
});
</script>

<template>
  <div class="score">
    <span>{{ label }}</span>
    <Heart />
  </div>
</template>

<style scoped>
  .score {
    padding: 12px 24px;
    border-radius: 36px;
    background-color: #CCE8FF;
    display: flex;
    align-items: center;
    justify-content: end;
    gap: 10px;
    font-size: 16px;
    line-height: 24px;
    font-weight: 700;
    color: #008BFE;
    min-width: 110px;
  }
  
</style>
