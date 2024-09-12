<template>
  <div :class="$style.medAI" id="medAI">
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
  @media screen and (max-width: 768px) {
    padding: 30px 16px;
    border-radius: 32px;
  }
}

.medAI::before {
  content: '';
  width: 800px;
  height: 130%;
  left: 44.7%;
  top: -8%;
  position: absolute;
  background-repeat: no-repeat;
  background-image: url('/public/cards.png');
}

@media screen and (max-width: 1440px) {
  .medAI::before {
    left: 50%;
    background-size: 100%;
    background-position: center top;
    top: 12%;
    width: 50%;
  }
}

@media screen and (max-width: 768px) {
  .medAI::before {
    left: 0;
    background-size: contain;
    background-position: center 75.5%;
    top: -8%;
    width: 100%;
  }
}

.heading {
  font-size: 60px;
  line-height: 66px;
  color: #7A62DB;
  margin-bottom: 15px;
  @media screen and (max-width: 768px) {
    font-size: 38px;
    margin-bottom: 22px;
    line-height: 46px;
  }
}

.text {
  margin-bottom: 69px;
  position: relative;
  z-index: 1;
  @media screen and (max-width: 768px) {
    display: none;
  }
}

.list {
  display: flex;
  gap: 16px;
  flex-direction: column;
  max-width: 490px;
  @media screen and (max-width: 768px) {
    gap: 18px;
    margin-bottom: 230px;
  }
}

.item {
  position: relative;
  padding-left: 39px;
  @media screen and (max-width: 768px) {
    font-size: 16px;
    line-height: 19px;
  }
}

.item::before {
  content: '';
  width: 100%;
  height: 100%;
  left: 0;
  position: absolute;
  background-repeat: no-repeat;
  background-image: url('/star.svg');
}
</style>
<script setup lang="ts">
</script>