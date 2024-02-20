<template>
  <header class="main-header">
    <div class="header-item img-number">
      <img src="/imgs/respakLogo.svg" alt="respak logo" class="header-logo" />
      <p class="header__text">+7 800 775 19 86</p>
    </div>

    <div class="header-item nav-button">
      <nav class="main-header__navigation">
        <ul class="navigation">
          <li class="navigation-item">
            <a href="#products" class="header__text">Продукты</a>
          </li>
          <li class="navigation-item">
            <a href="#about" class="header__text">О компании</a>
          </li>
        </ul>
      </nav>
      <button class="main-header__button">
        <img src="/imgs/header-button.png" alt="header button" />
      </button>
    </div>
  </header>
</template>

<script setup></script>

<style lang="scss" scoped>
header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  padding: 16px 0;
}

.header-logo {
  margin-right: 2rem;
}

.header-item {
  display: flex;
  align-items: center;
  /* width: 50%; */
}

.header__text {
  color: #141414;
  font-family: Montserrat;
  font-size: 1.5rem;
  font-weight: 700;
  text-decoration: none;
}
.navigation {
  list-style-type: none;
  display: flex;
  flex-direction: row;
}

/* .navigation-item {
  margin-right: 100px;
  a {
    @include underline;
    position: relative;
  }
} */

.nav-button {
  justify-content: space-between;
}

.main-header__button {
  width: fit-content;
  all: unset;
}
.main-header__button:hover {
  cursor: pointer;
}

.navigation-item {
  margin-right: 100px;
}
</style>
