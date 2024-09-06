<template>
  <div :class="$style.medicine">
    <div :class="$style.block">
      <h1 :class="$style.heading">Меняем подход  к&nbsp;медицине</h1>
      <p :class="$style.text">Разрабатываем приложения для профилактики заболеваний и улучшения качества жизни</p>
      <div :class="$style.select">
        <input placeholder="Ваш e-mail" />
      </div>
      <p :class="$style.text">Узнайте первыми о наших&nbsp;новостях<br/>и запусках приложений</p>
    </div>

    <img :class="$style.img" src="/public/mobile.png" alt="альтернативный текст">
  </div>
</template>

<style module>
.medicine {
  display: flex;
  padding-top: 17px;
  justify-content: space-between;
  gap: 32px;
}

.block {
  padding: 50px 60px;
  background-color: #F5F5F8;
  border-radius: 40px;
}

.heading {
  font-size: 96px;
  font-weight: 500;
  line-height: 96px;
  margin-bottom: 34px;
}

.img {
  height: 760px;
  border-radius: 40px;
}

.text {
  color: #73737A;
  font-size: 20px;
  font-weight: 500;
  line-height: 28px;
  max-width: 80%;
}

.select {
  background-color: #FFF;
  border-radius: 60px;
  margin: 119px 0 16px 0;
  color: #73737A;

  input {
    padding: 30px 32px;
    border-radius: 60px;
    font-size: 24px;
  }
}
</style>
<script setup lang="ts">
</script>