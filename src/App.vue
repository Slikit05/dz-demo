<script setup>
import Score from "./components/Score.vue";
import Card from "./components/Card.vue";

const data = {
  label: "100",
};
</script>

<template>
  <header class="header">
    <div class="header__wrapper">
      <span class="header__caption">ЗАПОМНИ СЛОВО</span>
      <Score v-bind="data" />
    </div>
  </header>
  <main class="main">
    <Card />
  </main>
</template>

<style scoped>
.header__wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 37px 62px;
}

.header__caption {
  font-size: 16px;
  line-height: 24px;
  font-weight: 700;
  letter-spacing: 0.12em;
}
.main {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  min-height: calc(100vh - 122px);
  padding: 62px;
}
</style>
