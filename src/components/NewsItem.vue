<template>
  <div class="news-item">
    <div class="img-wrapper">
      <img
        class="item-img"
        draggable="false"
        src="/imgs/news-item-picture.png"
        alt=""
      />
    </div>
    <div class="card-views">
      <div class="svg-wrapper">
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M19 12.5C19 14.985 15.866 17 12 17C8.134 17 5 14.985 5 12.5C5 10.015 8.134 8 12 8C15.866 8 19 10.015 19 12.5Z"
            stroke="white"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M13.75 12.4996C13.7716 13.1389 13.4429 13.7392 12.8925 14.0652C12.3422 14.3913 11.6578 14.3913 11.1075 14.0652C10.5571 13.7392 10.2284 13.1389 10.25 12.4996C10.2284 11.8603 10.5571 11.2601 11.1075 10.934C11.6578 10.6079 12.3422 10.6079 12.8925 10.934C13.4429 11.2601 13.7716 11.8603 13.75 12.4996V12.4996Z"
            stroke="white"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </div>

      <p>9012</p>
    </div>
    <div class="card-info">
      <svg
        width="8"
        height="8"
        viewBox="0 0 8 8"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <rect width="8" height="8" rx="2" fill="white" />
      </svg>
      <p>
        Какая-то значимая новость. Даже и не знаю, почему она такая интересная,
        но я бы нажал
      </p>
    </div>
    <div class="link-wrapper">
      <a class="" href="#">к новости</a>
      <div>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="41"
          height="16"
          viewBox="0 0 41 16"
          fill="none"
        >
          <path
            d="M40.7071 8.70711C41.0976 8.31658 41.0976 7.68342 40.7071 7.29289L34.3431 0.928932C33.9526 0.538408 33.3195 0.538408 32.9289 0.928932C32.5384 1.31946 32.5384 1.95262 32.9289 2.34315L38.5858 8L32.9289 13.6569C32.5384 14.0474 32.5384 14.6805 32.9289 15.0711C33.3195 15.4616 33.9526 15.4616 34.3431 15.0711L40.7071 8.70711ZM0 9H40V7H0V9Z"
            fill="black"
          />
        </svg>
      </div>
    </div>
    <div class="info">
      <p>13 августа 2023</p>
      <p>#аналитика</p>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.img-wrapper {
  width: fit-content;
  height: fit-content;
  position: relative;
  z-index: 0;
}

.news-item {
  position: relative;
  width: fit-content;
  height: fit-content;
  /* svg {
    position: absolute;
  }
  p {
    position: absolute;
  } */
}

.card-views {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  position: absolute;
  z-index: 2;
  background-color: rgba(29, 31, 34, 0.5);
  padding: 5px 35px;
  width: 100px;
  height: 24px;
  top: 0;
  right: 0;

  svg {
    /* position: absolute;
    left: 12px;
    bottom: 4px; */
  }
}

.card-info {
  display: flex;
  gap: 10px;
  position: absolute;
  top: 30px;
  left: 15px;
  z-index: 1;
  p {
    font-size: 12px;
    color: white;
    text-decoration: underline;
    max-width: 206px;
    max-height: 60px;
  }
}

.link-wrapper {
  z-index: 1;
  background-color: #fff;
  width: 100%;
  position: absolute;
  bottom: 0;
  height: 52px;
  display: flex;
  align-items: center;
  justify-content: center;
  a {
    text-decoration: none;
    color: black;
    font-weight: 500;
    flex: 1;
    text-align: center;
  }
  div {
    background-color: $text-light-green;
    height: 100%;
    width: 52px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
}

.item-img {
}
</style>
