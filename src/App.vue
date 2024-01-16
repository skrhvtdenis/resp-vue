<template>
  <div class="wrapper">
    <RespHeader />

    <FirstPage />

    <StoriesList />
  </div>
</template>

<script setup>
import RespHeader from "./components/RespHeader.vue";
import FirstPage from "./components/FirstPage.vue";
import StoriesList from "./components/StoriesList.vue";
</script>

<style lang="scss" scoped>
.wrapper {
  padding: 0 34px;
  margin: 0 auto;
  height: 100vh;
  background-color: #ffffff;
}
</style>
