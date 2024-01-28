<template>
  <section class="news">
    <h2 class="news__header">РЕСПАК:NEWS</h2>
    <div class="news__container">
      <!-- <div class="news__buttons">
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
      </div> -->
      <div class="news-list__grid">
        <!-- TODO: fix class bindings -->
        <NewsItem
          v-for="newItem in news"
          :key="newItem.id"
          :views="newItem.views"
          :headline="newItem.headline"
          :img="newItem.img"
          :date="newItem.date"
          :hashtag="newItem.hashtag"
          :class="
            newItem.id <= 3
              ? 'first-row'
              : newItem.id >= 10
              ? 'third-row'
              : 'second-row'
          "
        />
        <!-- <div class="big-news__grid third-row">
          <NewsItem v-for="bigNewsItem in bigNews"></NewsItem>
        </div> -->
      </div>
      <div class="third-row__flex">
        <div class="item-with-nav">
          <NewsItem class="active" />
          <p class="navigation-item">
            <a href="#" class="header__text"
              >все новости <img src="/imgs/arrow.png" alt=""
            /></a>
          </p>
        </div>
        <NewsItem />
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";
import NewsItem from "./NewsItem.vue";

const news = ref([
  {
    id: 1,
    views: 9012,
    headline:
      "Какая-то значимая новость. Даже и не знаю, почему она такая интересная, но я бы нажал",
    img: "/imgs/news-item-picture.png",
    date: "13 августа 2023",
    hashtag: "#аналитика",
  },
  {
    id: 1,
    views: 9012,
    headline:
      "Какая-то значимая новость. Даже и не знаю, почему она такая интересная, но я бы нажал",
    img: "/imgs/news-item-picture.png",
    date: "13 августа 2023",
    hashtag: "#аналитика",
  },
  {
    id: 1,
    views: 9012,
    headline:
      "Какая-то значимая новость. Даже и не знаю, почему она такая интересная, но я бы нажал",
    img: "/imgs/news-item-picture.png",
    date: "13 августа 2023",
    hashtag: "#аналитика",
  },
  {
    id: 4,
    views: 9012,
    headline:
      "Какая-то значимая новость. Даже и не знаю, почему она такая интересная, но я бы нажал",
    img: "/imgs/news-item-picture.png",
    date: "13 августа 2023",
    hashtag: "#аналитика",
  },
  {
    id: 5,
    views: 9012,
    headline:
      "Какая-то значимая новость. Даже и не знаю, почему она такая интересная, но я бы нажал",
    img: "/imgs/news-item-picture.png",
    date: "13 августа 2023",
    hashtag: "#аналитика",
  },
  {
    id: 6,
    views: 9012,
    headline:
      "Какая-то значимая новость. Даже и не знаю, почему она такая интересная, но я бы нажал",
    img: "/imgs/news-item-picture.png",
    date: "13 августа 2023",
    hashtag: "#аналитика",
  },
  {
    id: 6,
    views: 9012,
    headline:
      "Какая-то значимая новость. Даже и не знаю, почему она такая интересная, но я бы нажал",
    img: "/imgs/news-item-picture.png",
    date: "13 августа 2023",
    hashtag: "#аналитика",
  },
]);
const bigNews = ref([
  {
    id: 1,
    views: 9012,
    headline:
      "Какая-то значимая новость. Даже и не знаю, почему она такая интересная, но я бы нажал",
    img: "/imgs/news-item-picture.png",
    date: "13 августа 2023",
    hashtag: "#аналитика",
  },
  {
    id: 1,
    views: 9012,
    headline:
      "Какая-то значимая новость. Даже и не знаю, почему она такая интересная, но я бы нажал",
    img: "/imgs/news-item-picture.png",
    date: "13 августа 2023",
    hashtag: "#аналитика",
  },
]);
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
  align-items: center;
  background-color: #fff;
  border-radius: 160px;
  padding: 140px;
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

.news-list__grid {
  width: 100%;
  display: grid;
  grid-gap: 1rem;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: repeat(2, 1fr);
  justify-items: center;
  gap: 3rem 4.5rem;
  align-items: center;
  margin-bottom: 3rem;
}

.first-row {
  grid-column-start: span 4;
}

.second-row {
  grid-column-start: span 3;
  max-height: 300px;
}
/* .third-row {
  max-width: 785px;
  grid-column-start: span 6;
} */

.third-row__flex {
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  gap: 4.5rem;

  .item-with-nav {
    display: flex;
    flex-direction: column;
    width: 100%;

    p {
      margin-top: 40px;
    }
  }
}
</style>
