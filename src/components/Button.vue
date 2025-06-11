<script setup></script>

<template>
  <button class="button">
    <div>
      <slot name="icon" />
    </div>
    <slot />
  </button>
</template>

<style scoped>
  .button {
    border: none;
    border-radius: 100px;
    background-color: var(--color-bg-button);
    color: var(--color-btn);
    font-weight: 400;
    padding: 16px 10px;
    font-size: 24px;
    line-height: 36px;
    cursor: pointer;
    transition: background-color 0.3s ease-in-out;
    max-width: 335px;
    width: 100%;
  }

  .button:hover {
    background-color: var(--color-bg-hover-button);
  }
</style>