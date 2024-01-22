<template>
  <div class="news-item">
    <div class="card-views">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="16"
        height="11"
        viewBox="0 0 16 11"
        fill="none"
      >
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M15 5.5C15 7.985 11.866 10 8 10C4.134 10 1 7.985 1 5.5C1 3.015 4.134 1 8 1C11.866 1 15 3.015 15 5.5Z"
          stroke="white"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M9.75 5.49962C9.77161 6.13895 9.44287 6.73918 8.89253 7.06524C8.34218 7.39131 7.65782 7.39131 7.10747 7.06524C6.55712 6.73918 6.22838 6.13895 6.25 5.49962C6.22838 4.8603 6.55712 4.26007 7.10747 3.934C7.65782 3.60794 8.34218 3.60794 8.89253 3.934C9.44287 4.26007 9.77161 4.8603 9.75 5.49962V5.49962Z"
          stroke="white"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
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
    <img src="/imgs/news-item-picture.png" alt="" />
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.news-item {
  width: fit-content;
  height: fit-content;
  position: relative;
  svg {
    position: absolute;
  }
  p {
    position: absolute;
  }
}

.card-views {
  position: relative;
  z-index: 1;
  background-color: rgba(29, 31, 34, 0.5);
  padding: 5px 35px;
  width: 100px;
  height: 24px;
  svg {
    position: absolute;
    left: 12px;
    bottom: 4px;
  }
}
</style>
