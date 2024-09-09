<template>
  <div :class="$style.medicine">
    <div :class="$style.block">
      <h1 :class="$style.heading">Меняем подход к&nbsp;медицине</h1>
      <p :class="$style.text">Разрабатываем приложения для профилактики заболеваний и улучшения качества жизни</p>
      <div :class="$style.select">
        <input placeholder="Ваш e-mail" />
        <button :class="$style.button">Подписаться</button>
      </div>
      <p :class="$style.text">Узнайте первыми о наших&nbsp;новостях<br/>и запусках приложений</p>
    </div>

    <img :class="$style.img" src="/public/mobile.png" alt="альтернативный текст">
  </div>
</template>

<style module>
.medicine {
  display: flex;
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
  max-width: 300px;
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
  display: flex;
  justify-content: space-between;

  input {
    padding: 30px 32px;
    border-radius: 60px;
    font-size: 24px;
    width: 100%;
  }
}

.button {
  font-size: 20px;
  font-weight: 700;
  line-height: 22px;
  color: #fff;
  border-radius: 60px;
  background: #111114;
  padding: 23px 36px;
  margin: 8px;
}
</style>