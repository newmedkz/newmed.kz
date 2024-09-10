<template>
  <div :class="$style.container">
    <left-panel />
    <div :class="$style.view">
      <medicine />
      <services />
      <med-a-i />
      <team />
      <p :class="$style.info">ИНН 7710641442; ОГРН 5067746338732; адрес: РФ, 123056, г. Москва,<br/> Грузинский пер., д 3А.</p>
    </div>
  </div>
</template>

<script setup lang="ts">
import LeftPanel from "~/components/LeftPanel.vue";
import Services from "~/components/Services.vue";

</script>

<style module>
body {
  height: auto;
  font-family: 'Manrope', 'MTSSans', BlinkMacSystemFont, 'Roboto', 'Segoe UI',
  'Helvetica Neue', Arial, sans-serif;
  color: #111114;
  margin: 0;
  width: 100%;
  max-width: 100%;
  overflow-x: hidden;
}

* {
  box-sizing: border-box;
  font-weight: 400;
}

p, h1, ul, h3 {
  margin: 0;
  padding: 0;
  list-style-type: none;
}

input, button {
  border: 0;
  outline: 0;
}

.container {
  max-width: 1920px;
  padding: 24px 24px 60px 60px;
  margin: 0 auto;
  width: 100%;
  display: flex;
  justify-content: space-between;
  @media screen and (max-width: 768px) {
    flex-direction: column;
    padding: 8px 16px 70px 16px;
    max-width: 375px;
  }
}

.view {
  max-width: 1455px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: end;
  gap: 40px;
  @media screen and (max-width: 768px) {
    max-width: 343px;
    gap: 20px;
  }
}

.info {
  color: #CCCCCC;
  font-size: 16px;
  margin: 4px 25px 0 0;
  @media screen and (min-width: 768px) {
    display: none;
  }
}

</style>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Manrope:wght@200..800&display=swap" rel="stylesheet">
