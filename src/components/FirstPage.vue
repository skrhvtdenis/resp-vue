<template>
  <section class="first_page">
    <div class="first-page__content">
      <div class="content__item item-info">
        <h1 class="info-name linear-wipe">РЕСПАК</h1>
        <h3 class="info-description">
          Платформа цифровых<br />
          сервисов в АПК
        </h3>
        <p class="info-small-text">
          Решение внесено в реестр отечественного ПО №4398 от 16.04.2018
        </p>
        <nav class="info-links">
          <a href="https://t.me/respakteam">
            <img src="/imgs/telegram-logo.png" alt="respak telegram link" />
          </a>
          <img src="/imgs/apple-logo.png" alt="apple-logo" href="#" />
          <img src="/imgs/playmarket-logo.png" alt="playmarket-logo" href="#" />
        </nav>
      </div>
      <div class="content__item item-pic">
        <!-- <img src="/imgs/girl-picture.png" alt="girl" class="content-img" /> -->
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped>
.first-page__content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  min-height: 88vh;
}

.item-info {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding-bottom: 75px;
}

.info-name {
  color: $text-light-green;
  font-size: 8.125rem;
  font-weight: 900;
  margin-bottom: 95px;
}

.info-description {
  color: #000;
  font-size: 2.875rem;
  font-weight: 900;
  margin-bottom: 62px;
}

.info-small-text {
  color: #979797;
  font-size: 1.25rem;
  font-weight: 500;

  margin-bottom: 62px;
}

.info-links img {
  margin-right: 35px;
}
.info-links a {
  text-decoration: none;
}
.content-img {
  max-height: 795px;
}

@media screen and (max-width: 700px) {
  .info-name {
    font-size: 6rem;
  }
  .info-description {
    font-size: 2rem;
  }
}
@media screen and (max-width: 526px) {
  .info-name {
    font-size: 5rem;
  }
  .info-description {
    font-size: 1.5rem;
  }
  .info-small-text {
    font-size: 1rem;
  }
}

// GRADIENT
.linear-wipe {
  background: linear-gradient(
    to right,
    #35cf72 20%,
    #01925a 40%,
    #01925a 60%,
    #35cf72 80%
  );
  background-size: 200% auto;

  color: #000;
  background-clip: text;
  text-fill-color: transparent;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;

  animation: shine 6s linear infinite;
  @keyframes shine {
    to {
      background-position: 200% center;
    }
  }
}
</style>
