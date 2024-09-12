<template>
  <div :class="$style.team" id="team">
    <h3 :class="$style.heading">Команда</h3>
    <ul :class="$style.list">
      <li :class="$style.item" v-for="item in list" :key="item.id"
          :style="{ backgroundImage: `url( ${item.id} )` }"
      >
        <p :class="$style.name">{{item.name}}</p>
        <p :class="$style.position">{{item.position}}</p>
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">

const list = [
  {id: '/1.png', name: 'Пилипчук Александр', position: 'Ген. директор'},
  {id: '/2.jpg', name: 'Георгий Лондаридзе', position: 'CTO'},
  {id: '/3.png', name: 'Владислав Торгов', position: 'Architect'},
  {id: '/4.png', name: 'Алёна Лопухова', position: 'CPO'},
  {id: '/5.png', name: 'Полина Фурманова', position: 'Delivery Lead'},
];
</script>

<style module>
.team {
  border-radius: 40px;
  padding: 50px 60px;
  width: 100%;
  font-size: 20px;
  line-height: 24px;
  border: 1.5px solid #DCDCE5;
  @media screen and (max-width: 768px) {
    padding: 30px 16px 16px 16px;
    border-width: 1px;
    border-radius: 32px;
  }
}

.heading {
  font-size: 60px;
  line-height: 66px;
  margin-bottom: 33px;
  @media screen and (max-width: 768px) {
    font-size: 38px;
    line-height: 45.6px;
    margin-bottom: 16px;
  }
}

.list {
  display: flex;
  gap: 19px;
  flex-wrap: wrap;
  @media screen and (max-width: 768px) {
    gap: 8px;
  }
}

.item {
  width: 251px;
  height: 287px;
  border-radius: 32px;
  background: #F5F5F8;
  padding: 0 24px 20px 24px;
  display: flex;
  flex-direction: column;
  justify-content: end;
  background-repeat: no-repeat;
  background-position: top center;
  @media screen and (max-width: 768px) {
    width: 150px;
    padding: 0 15px 18px 15px;
    height: 182px;
    background-size: contain;
    border-radius: 19px;
  }
}


.name {
  font-size: 24px;
  line-height: 31.2px;
  margin-bottom: 8px;
  max-width: 80%;
  @media screen and (max-width: 768px) {
    font-size: 16px;
    margin-bottom: 2px;
    max-width: 100%;
    line-height: 20px;
  }
}

.position {
  font-size: 16px;
  color: #73737A;
  @media screen and (max-width: 768px) {
  font-size: 12px;
  line-height: 15px;
  }
}
</style>
