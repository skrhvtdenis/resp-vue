<template>
  <div class="container">
    <div class="flex-container">
      <div class="left">
        <p>более</p>
        <p class="number">20</p>
        <p>регионов</p>
      </div>
      <div class="right">
        <p class="big-text black">Желаете</p>
        <p class="big-text">присоединиться?</p>
      </div>
    </div>
    <p class="navigation-item">
      <a>&ensp;Напишите нам <img src="/imgs/arrow.png" alt="" /></a>
    </p>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.container {
}

.flex-container {
  display: flex;
  justify-content: start;
  align-items: center;
}

.big-text {
  color: $text-light-green;
  font-size: 8rem;
  font-weight: 800;
}

.number {
  color: $text-light-green;
  font-size: 15rem;
  font-weight: 800;
}

.black {
  color: black;
}

.navigation-item {
  grid-area: d;
}
</style>
