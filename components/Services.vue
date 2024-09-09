<template>
  <div :class="$style.services">
    <h3 :class="$style.heading">Кто мы такие?</h3>
    <div :class="$style.wrapper">
      <p :class="$style.text">Мы предлагаем передовые цифровые решения для отслеживания состояния здоровья. Наши продукты помогают следить за самочувствием и предотвращать риски развития заболеваний.</p>
      <p :class="$style.text">Следите за обновлениями и внедряйте новых персональных помощников в свой здоровый образ жизни</p>
    </div>
  </div>
</template>

<style module>
.services {
  border-radius: 40px;
  background: #32323B;
  padding: 60px;
  width: 100%;
  @media screen and (max-width: 768px) {
    padding: 30px 16px;
  }
}

.heading {
  font-size: 60px;
  font-weight: 400;
  line-height: 66px;
  color: #fff;
  background-image: url('/public/services.png');
  padding-bottom: 165px;
  border-bottom: 1px solid #73737A;
  margin-bottom: 42px;
  background-position: 73px -14px;
  background-repeat: no-repeat;
  @media screen and (max-width: 768px) {
    font-size: 38px;
    background-image: url('/public/services2.png');
    background-position: bottom center;
    margin-bottom: 23px;
    background-size: 100%;
    padding-bottom: 112px;
  }
}

.wrapper {
  display: flex;
  gap: 145px;
  @media screen and (max-width: 768px) {
    flex-direction: column;
    gap: 16px;
  }
}

.text {
  color: #DCDCE5;
  font-size: 20px;
  font-weight: 500;
  line-height: 24px;
  max-width: 430px;
  @media screen and (max-width: 768px) {
    font-size: 16px;
    font-weight: 400;
  }
}
</style>