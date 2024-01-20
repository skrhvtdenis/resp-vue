<template>
  <section class="products">
    <h2 class="green-thingy" id="products">Наши продукты</h2>
    <div class="products__container">
      <div class="products__container-item">
        <p class="product-name">ИС.РЕСПАК</p>
        <div class="product-info__container">
          <p class="main-text">Региональная<br />система</p>
          <hr />
          <div class="img__container">
            <img src="/imgs/Cube-icon.svg" alt="" />
            <img src="/imgs/Dashboard 3-icon.svg" alt="" />
          </div>
          <p class="little-text">Микросервисная архитектура</p>
        </div>
        <p class="main-text">
          Решение для сельского хозяйства, обеспечивающее цифровое
          взаимодействие органов власти и сельхозтоваропроизводителей региона.
        </p>
      </div>
      <div class="products__container-item">
        <div class="name__container">
          <p class="product-name__small">господдержка</p>
          <p class="product-name__big">АПК НСО</p>
        </div>
        <div class="product-info__container">
          <p class="main-text">mobile APP</p>
          <hr />
          <div class="img__container">
            <img src="/imgs/aple.svg" alt="" />
            <img src="/imgs/market.svg" alt="" />
            <img src="/imgs/rustore.png" alt="" />
          </div>
        </div>
        <p class="main-text">
          Мобильное приложение для ИС.РЕСПАК для региона Новосибирск
        </p>
      </div>

      <div class="products__container-item">
        <p class="product-name">ИС ЦС АПК</p>
        <div class="product-info__container">
          <p class="main-text">Федеральная<br />система</p>
          <hr />
          <div class="img__container">
            <img src="/imgs/Cube-icon.svg" alt="" />
            <img src="/imgs/Dashboard 3-icon.svg" alt="" />
          </div>
          <p class="little-text">Микросервисная архитектура</p>
        </div>
        <p class="main-text">
          Че-то для чего, никто не знает для чего вообще, но че-то федерального
          уровня
        </p>
      </div>
      <p class="navigation-item final-link">
        <a href="#" class="header__text"
          >все проекты <img src="/imgs/arrow.png" alt=""
        /></a>
      </p>
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped>
.products__container {
  background-color: #fff;
  border-radius: 160px;
}

.products__container-item {
  padding: 58px 150px 150px 58px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.product-info__container {
  width: 250px;
}

.product-info__container p {
  text-align: center;
}

.img__container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 27px;
}

.product-info__container hr {
  background-color: #000;
  border: none;
  height: 3px;
  margin-top: 8px;
  margin-bottom: 12px;
}

.main-text {
  max-width: 420px;
  color: #1d1f22;
  font-size: 1.5rem;
  font-weight: 500;
}

.product-name {
  color: #1d1f22;
  font-size: 8.125rem;
  font-weight: 800;
}

.product-name__small {
  color: #35cf72;
  font-size: 6.25rem;
  font-weight: 800;
}
.product-name__big {
  color: #35cf72;
  font-size: 128px;
  font-weight: 800;
}
.final-link {
  text-align: center;
  padding-bottom: 150px;
}
</style>
