<template>
  <div :class="$style['left-panel']">
    <div>
    <img :class="$style.img" src="public/logo.svg" alt="Логотип">
    <nav :class="$style.nav">
      <ul :class="$style.list">
        <li><a href="/" :class="$style.link">Главная</a></li>
        <li :class="$style.item"><a>О компании</a></li>
        <li :class="$style.item"><a>Наши проекты</a></li>
        <li :class="$style.item"><a>Команда</a></li>
      </ul>
    </nav>
    </div>
    <p :class="$style.info">ИНН 231240027989; ОГРН&nbsp;231240027989; адрес:&nbsp;Казахстан, город Алматы, Медеуский район, улица Зенкова, дом 32, кв. 1, почтовый индекс 050000</p>
  </div>
</template>

<script setup lang="ts">
</script>

<style module>
.left-panel {
  max-width: 275px;
  padding-top: 30px;
  position: sticky;
  top: 0;
  height: 95vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  @media screen and (max-width: 768px) {
    height: auto;
    position: static;
    margin-bottom: 13px;
  }
}

.nav {
  width: max-content;
  @media screen and (max-width: 768px) {
    display: none;
  }
}

.list {
  display: flex;
  flex-direction: column;
  gap: 31px;
  margin-top: 70px;
  font-size: 20px;
}

.item {
  color: #919199;
}

.link {
  color: #111114;
  text-decoration: none;
}

.info {
  color: #CCCCCC;
  @media screen and (max-width: 768px) {
    display: none;
  }
}

.img {
  @media screen and (max-width: 768px) {
    width: 163px;
  }
}
</style>
