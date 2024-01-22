<template>
  <section class="news">
    <h2 class="news__header">РЕСПАК:NEWS</h2>
    <div class="news__container">
      <div class="news__buttons">
        <button class="page-btn btn-back">
          <img src="/imgs/Arrow_Left_5.svg" class="circle" alt="arrow-left" />
        </button>
        <div class="news-page__number">
          <hr />
          <p class="pages-number"><span class="current-page">01 </span>/ 08</p>
        </div>
        <button class="page-btn btn-next">
          <img
            src="/imgs/arrow-right-act.svg"
            class="circle"
            alt="arrow-right"
          />
        </button>
      </div>
      <div class="news-container">
        <NewsItem />
      </div>
    </div>
  </section>
</template>

<script setup>
import NewsItem from "./NewsItem.vue";
</script>

<style lang="scss" scoped>
.news__header {
  margin-top: 175px;
  margin-bottom: 46px;
  margin-right: 144px;
  text-align: right;
  position: relative;
}

/* .news__header::before {
} */

.news__container {
  display: flex;
  flex-direction: column;
  background-color: #fff;
  border-radius: 160px;
  padding: 150px;
}

.news__buttons {
  max-width: 340px;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
}

.news-page__number {
  margin: 0 36px;
}

.news__buttons hr {
  width: 250px;
  height: 1px;
}

.pages-number {
  font-size: 0.75rem;
  font-weight: 600;
}

.current-page {
  color: $text-light-green;
}

.page-btn {
  all: unset;
}

.page-btn:hover {
  cursor: pointer;
}

.circle {
  width: 68px;
  height: 68px;
  border-radius: 50%;
  background-color: #000000;
  padding: 9px;
  opacity: 0.8;
}
.circle:hover {
  opacity: 1;
}
</style>
