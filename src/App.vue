<template>
  <div class="bg">
    <div class="wrapper">
      <RespHeader />

      <FirstPage />

      <StoriesList />
    </div>

    <ProductsList />

    <NewsList class="mb" />

    <MobileApp class="mb" />

    <MapInfo />
  </div>
</template>

<script setup>
import RespHeader from "./components/RespHeader.vue";
import FirstPage from "./components/FirstPage.vue";
import StoriesList from "./components/StoriesList.vue";
import ProductsList from "./components/ProductsList.vue";
import NewsList from "./components/NewsList.vue";
import MobileApp from "./components/MobileApp.vue";
import MapInfo from "./components/MapInfo.vue";
</script>

<style lang="scss">
.wrapper {
  padding: 0 34px;
  margin: 0 auto;
  height: 100vh;
  /* TODO: FIX MARGIN-BOTTOM LATER */
  margin-bottom: 300px;
}

.mb {
  margin-bottom: 150px;
}
</style>
