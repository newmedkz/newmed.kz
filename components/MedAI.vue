<template>
  <div :class="$style.medAI">
    <h3 :class="$style.heading">Приложение MedAI</h3>
    <p :class="$style.text">Персональный помощник в снижении рисков заболеваний</p>
    <ul :class="$style.list">
      <li :class="$style.item">
        Анализ состояния каждого органа и алгоритмы оценки рисков по анализам
      </li>
      <li :class="$style.item">
        Исследование родинок с помощью<br/>технологии Skinive
      </li>
      <li :class="$style.item">
        Отслеживание активности с учетом состояния здоровья и персональные рекомендации
      </li>
      <li :class="$style.item">
        Женский календарь и персональный мониторинг циклов
      </li>
    </ul>
  </div>
</template>

<style module>
.medAI {
  position: relative;
  border-radius: 40px;
  background-color: #D6CCFF;
  padding: 60px 60px 41px 60px;
  width: 100%;
  font-size: 20px;
  font-weight: 500;
  line-height: 24px;
  color: #111114;
}

.medAI::before {
  content: '';
  width: 100%;
  height: 130%;
  left: 44.7%;
  top: -8%;
  position: absolute;
  background-repeat: no-repeat;
  background-image: url('/public/cards.png');
}

.heading {
  font-size: 60px;
  line-height: 66px;
  color: #7A62DB;
  margin-bottom: 15px;
}

.text {
  margin-bottom: 69px;
}

.list {
  display: flex;
  gap: 16px;
  flex-direction: column;
  max-width: 490px;
}

.item {
  position: relative;
  padding-left: 39px;
}

.item::before {
  content: '';
  width: 100%;
  height: 100%;
  left: 0;
  top: -6%;
  position: absolute;
  background-repeat: no-repeat;
  background-image: url('/star.svg');
}
</style>
<script setup lang="ts">
</script>