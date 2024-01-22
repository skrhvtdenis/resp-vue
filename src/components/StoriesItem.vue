<template>
  <div class="stories-item">
    <p class="stories__date stories__text">{{ storie.date }}</p>
    <div class="stories__picture">
      <img
        draggable="false"
        src="/imgs/stories-picture-1.svg"
        alt=""
        class="stories--img"
      />
    </div>
    <p class="stories__date stories__text">
      {{ storie.text }}
    </p>
  </div>
</template>

<script setup>
defineProps({
  storie: Object,
});
</script>

<style lang="scss" scoped>
.stories-item {
  max-width: 336px;
}

.stories__picture {
  margin: 20px 0;
}
.stories--img {
  width: 336px;
  height: 201px;
  background: radial-gradient(
        circle at 100% 100%,
        #ffffff 0,
        #ffffff 16px,
        transparent 16px
      )
      0% 0%/20px 20px no-repeat,
    radial-gradient(circle at 0 100%, #ffffff 0, #ffffff 16px, transparent 16px)
      100% 0%/20px 20px no-repeat,
    radial-gradient(circle at 100% 0, #ffffff 0, #ffffff 16px, transparent 16px)
      0% 100%/20px 20px no-repeat,
    radial-gradient(circle at 0 0, #ffffff 0, #ffffff 16px, transparent 16px)
      100% 100%/20px 20px no-repeat,
    linear-gradient(#ffffff, #ffffff) 50% 50% / calc(100% - 8px)
      calc(100% - 40px) no-repeat,
    linear-gradient(#ffffff, #ffffff) 50% 50% / calc(100% - 40px)
      calc(100% - 8px) no-repeat,
    linear-gradient(90deg, #01ac6a 0%, rgba(1, 172, 106, 0.65) 100%);
  border-radius: 20px;
  padding: 4px;
  box-sizing: border-box;
}

.stories__text {
  text-align: center;
  color: #1d1f22;
  font-size: 0.75rem;
  font-weight: 500;
}
</style>
