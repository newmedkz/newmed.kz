<template>
  <div :class="$style.medicine" id="medicine">
    <div :class="$style.block">
      <h1 :class="$style.heading">Меняем подход к&nbsp;медицине</h1>
      <p :class="$style.text">Разрабатываем приложения для профилактики заболеваний и улучшения качества жизни</p>
      <div :class="$style.search">
        <input placeholder="Ваш e-mail" />
        <button :class="$style.button">Подписаться</button>
      </div>
      <p :class="$style.text">Узнайте первыми о наших&nbsp;новостях и&nbsp;запусках&nbsp;приложений</p>
    </div>

    <img :class="$style.img" src="/public/mobile.png" alt="Картинка мобильного телефона">
  </div>
</template>

<style module>
.medicine {
  display: flex;
  justify-content: space-between;
  gap: 32px;
  @media screen and (max-width: 768px) {
    flex-direction: column;
    gap: 20px;
  }
}

.block {
  padding: 50px 60px;
  background-color: #F5F5F8;
  border-radius: 40px;
  @media screen and (max-width: 768px) {
    padding: 30px 16px;
    border-radius: 32px;
  }
}

.heading {
  font-size: 96px;
  line-height: 96px;
  margin-bottom: 34px;
  max-width: 300px;

  @media screen and (max-width: 1440px) {
    font-size: 80px;
    line-height: 80px;
  }

  @media screen and (max-width: 1360px) {
    font-size: 60px;
    line-height: 60px;
  }

  @media screen and (max-width: 768px) {
    font-size: 38px;
    line-height: 120%;
    margin-bottom: 19px;
  }
}

.img {
  height: 760px;
  border-radius: 40px;
  @media screen and (max-width: 1440px) {
    width: 50%;
    max-height: 700px;
  }
  @media screen and (max-width: 768px) {
    max-height: 400px;
    border-radius: 21px;
    width: 100%;
  }
}

.text {
  color: #73737A;
  font-size: 20px;
  line-height: 28px;
  max-width: 80%;
  @media screen and (max-width: 1440px) {
    max-width: 100%;
  }
  @media screen and (max-width: 768px) {
    font-size: 18px;
    line-height: 25px;
  }
}

.search {
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

  @media screen and (max-width: 1440px) {
    margin: 66px 0 16px 0;
  }

  @media screen and (max-width: 1360px) {
    margin: 66px 0 16px 0;
    input {
      padding: 18px 20px;
      font-size: 16px;
    }
  }
}

.button {
  font-size: 20px;
  font-weight: 600;
  line-height: 22px;
  color: #fff;
  border-radius: 60px;
  background: #111114;
  padding: 23px 36px;
  margin: 8px;
  @media screen and (max-width: 1360px) {
    font-size: 16px;
    padding: 13px 25px;
    margin: 4px;
    line-height: 17px;
  }
}
</style>