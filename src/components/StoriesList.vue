<template>
  <div class="stories-wrapper">
    <div class="svg-hover">
      <svg
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M22 12C22 6.48 17.52 2 12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12ZM9.35 11.65L12.14 8.86C12.46 8.54 13 8.76 13 9.21L13 14.8C13 15.25 12.46 15.47 12.15 15.15L9.36 12.36C9.16 12.16 9.16 11.84 9.35 11.65Z"
          fill="#E7E7E7"
        />
      </svg>
    </div>
    <div class="stories__container">
      <StoriesItem class="item" />
      <StoriesItem class="item" />
      <StoriesItem class="item" />
      <StoriesItem class="item" />
    </div>
    <div class="svg-hover">
      <svg
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C6.48 2 2 6.48 2 12ZM14.65 12.35L11.86 15.14C11.54 15.46 11 15.24 11 14.79L11 9.2C11 8.75 11.54 8.53 11.85 8.85L14.64 11.64C14.84 11.84 14.84 12.16 14.65 12.35Z"
          fill="#E7E7E7"
        />
      </svg>
    </div>
  </div>
</template>

<script setup>
import StoriesItem from "./StoriesItem.vue";
</script>

<style lang="scss" scoped>
.svg-hover {
  svg path {
    fill: #e7e7e7;
    opacity: 0.6;
  }
  &:hover {
    cursor: pointer;
    svg path {
      opacity: 1;
    }
  }
}

.stories-wrapper {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}
.item {
  margin-right: 100px;
}

.item:last-child {
  margin-right: 0;
}

.stories__container {
  margin: 0 auto;
  max-width: 1680px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
