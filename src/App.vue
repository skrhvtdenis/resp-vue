<template>
  <div class="bg">
    <div class="wrapper">
      <RespHeader />

      <FirstPage />

      <StoriesList />

      <ProductsList />
    </div>
  </div>
</template>

<script setup>
import RespHeader from "./components/RespHeader.vue";
import FirstPage from "./components/FirstPage.vue";
import StoriesList from "./components/StoriesList.vue";
import ProductsList from "./components/ProductsList.vue";
</script>

<style lang="scss">
.wrapper {
  padding: 0 34px;
  margin: 0 auto;
  height: 100vh;
}
</style>
