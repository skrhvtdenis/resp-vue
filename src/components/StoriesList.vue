<template>
  <div class="stories-wrapper" @mouseup="dragStop">
    <!-- <div class="svg-hover" @click="changeCard(-itemWidth)">
      <svg
        @click="reduceCur"
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
    </div> -->
    <div
      @mousemove="dragging"
      @mousedown="dragStart"
      ref="carousel"
      class="stories__container"
      :class="{ dragging: isDragging }"
    >
      <StoriesItem
        ref="storiesRefs"
        class="item active"
        v-for="(storie, i) in stories"
        v-bind:style="{ transform: 'translateX(0%)' }"
        :key="storie.id"
        :storie="storie"
      />
    </div>
    <!-- <div class="svg-hover" @click="changeCard(itemWidth)">
      <svg
        @click="addCur"
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
    </div> -->
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";
import StoriesItem from "./StoriesItem.vue";

const stories = ref([
  {
    id: 1,
    date: "0",
    text: "ФГИС Зерно, мы запускаем новый модуль! Смотрите подробности",
    img: "/imgs/stories-picture-1.svg",
  },
  {
    id: 2,
    date: "1",
    text: "ФГИС Зерно, мы запускаем новый модуль! Смотрите подробности",
    img: "/imgs/stories-picture-1.svg",
  },
  {
    id: 3,
    date: "2",
    text: "ФГИС Зерно, мы запускаем новый модуль! Смотрите подробности",
    img: "/imgs/stories-picture-1.svg",
  },
  {
    id: 4,
    date: "3",
    text: "ФГИС Зерно, мы запускаем новый модуль! Смотрите подробности",
    img: "/imgs/stories-picture-1.svg",
  },
  {
    id: 5,
    date: "4",
    text: "ФГИС Зерно, мы запускаем новый модуль! Смотрите подробности",
    img: "/imgs/stories-picture-1.svg",
  },
  {
    id: 6,
    date: "5",
    text: "ФГИС Зерно, мы запускаем новый модуль! Смотрите подробности",
    img: "/imgs/stories-picture-1.svg",
  },
]);
const carousel = ref(null);

const storiesRefs = ref([]);

const itemWidth = ref(500);

const startX = ref();
const startScrollLeft = ref();

const isDragging = ref(false);

const dragStart = (e) => {
  isDragging.value = true;

  // Records the initial cursor and scroll position of the carousel
  startX.value = e.pageX;
  startScrollLeft.value = carousel.value.scrollLeft;
};
const dragStop = () => {
  isDragging.value = false;
};

const dragging = (e) => {
  if (!isDragging.value) return; // if isDragging is false return from here
  // Updates the scroll positio of the carousel based on the cursor movement
  carousel.value.scrollLeft = startScrollLeft.value - (e.pageX - startX.value);
};

const changeCard = function (direction) {
  console.log(direction);
  carousel.value.scrollLeft += direction;
};

onMounted(() => {
  console.log(carousel.value);
  console.log(itemWidth.value);
  console.log(storiesRefs);
});

/* watch(isDragging, () => {}); */
</script>

<style lang="scss" scoped>
.active {
  display: block;
}

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
  margin: 0 auto;
  width: 100%;
  display: flex;
  align-items: center;
  /*  width: 1826px; */
  /* justify-content: center; */
}

.item:last-child {
  margin-right: 0;
}

.stories__container {
  display: grid;
  grid-auto-flow: column;
  grid-auto-columns: calc((100% / 3));
  gap: 1.5rem;
  justify-items: center;
  /*  max-width: 1680px; */
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  scroll-behavior: smooth;
  scrollbar-width: none;
}

.stories__container::-webkit-scrollbar {
  display: none;
}

.stories__container.dragging {
  /* scroll-snap-type: none; */
  scroll-behavior: auto;
}

@media (max-width: 1500px) {
  .stories__container {
    grid-auto-columns: calc(100% / 3);
  }
}
@media (max-width: 1200px) {
  .stories__container {
    grid-auto-columns: calc(100% / 4);
  }
}
</style>
