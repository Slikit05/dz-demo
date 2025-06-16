<script setup>
import NoIcon from "../icons/NoIcon.vue";
import YesIcon from "../icons/YesIcon.vue";

const turnOver = (event) => {
  console.log('Перевернули')
};

const status = (event) => {
  console.log('Статут изменился')
};
</script>

<template>
  <div class="card" @click="turnOver()" @change="status()">
    <div class="card__block card__block_front">
      <div class="card__wrap">
        <div class="card__up">
          <span class="card__number">01</span>
          <div class="card__icon"></div>
        </div>
        <div class="card__middle">
          <span class="card__text">unadmitted</span>
        </div>
        <div class="card__bottom">
          <span class="card__state">ПЕРЕВЕНУТЬ</span>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card__block {
  padding: 28px 19px;
  overflow: hidden;
  border-radius: 16px;
  box-shadow: 0px 0px 16px 0px rgba(0, 0, 0, 0.1);
  background-color: #fff;
  height: 100%;
  cursor: pointer;
  transition: box-shadow 0.3s ease-in-out;
}

.card__block:hover {
  box-shadow: 0px 0px 16px 0px rgba(0, 0, 0, 0.1), 10px 10px 10px 0px #0000000d;
}

.card__wrap {
  position: relative;
  padding: 16px;
  border-radius: 12px;
  border: 1px solid #cce8ff;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  color: #000;
  height: 100%;
}

.card__up {
  width: 100%;
}

.card__number {
  background-color: #fff;
  display: inline-block;
  font-size: 14px;
  line-height: 1;
  transform: translateY(-26px);
  padding: 0 1px;
}

.card__middle {
  width: 100%;
}

.card__text {
  display: block;
  text-align: center;
  font-size: 14px;
  line-height: 1;
}

.card__bottom {
  max-width: 160px;
  background-color: #fff;
  padding: 0 4px;
  transform: translateY(26px);
}

.card__state {
  font-size: 12px;
  line-height: 18px;
  font-weight: 700;
  letter-spacing: 0.12em;
}
</style>
