<template>
  <div :class="$style.container">
    <left-panel/>
    <div :class="$style.view">
      <medicine/>
      <div :class="$style.services">

      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import LeftPanel from "~/components/LeftPanel.vue";
</script>

<style module>
body {
  height: auto;
  font-family: 'MTSSans', BlinkMacSystemFont, 'Roboto', 'Segoe UI',
  'Helvetica Neue', Arial, sans-serif;
  color: #111114;
  margin: 0;
}

p, h1, ul {
  margin: 0;
  padding: 0;
}

input {
  border: 0;
  outline: 0;
}

.container {
  max-width: 1920px;
  padding: 0 24px;
  margin: 0 auto;
  width: 100%;
  @media screen and (min-width: 768px) {
    display: flex;
  }
}

.view {
  width: 100%;
  display: flex;
  justify-content: end;
}

.services {
  background-color: grey;
  background-image: url('/public/services.png');
}
</style>