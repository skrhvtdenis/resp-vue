<template>
  <div class="bg">
    <div class="container">
      <div class="left-col">
        <div class="page-head">
          <p class="app-name">Mobile App</p>

          <h1>Lorem, ipsum dolor.</h1>
          <h1>Господдержка АПК НСО</h1>

          <p>Мобильное приложение для ИС.РЕСПАК для региона Новосибирск</p>
        </div>

        <div class="description-container">
          <div class="description-item">
            <img src="/imgs/Hands001.png" alt="" />
            <p>Lorem ipsum dolor sit amet, consectetur</p>
          </div>
          <div class="description-item">
            <img src="/imgs/Hands002.png" alt="" />
            <p>Lorem ipsum dolor sit amet, consectetur</p>
          </div>
          <div class="description-item">
            <img src="/imgs/Hands003.png" alt="" />
            <p>Lorem ipsum dolor sit amet, consectetur</p>
          </div>

          <p class="navigation-item">
            <a href="#" class=""
              >все проекты <img src="/imgs/arrow.png" alt=""
            /></a>
          </p>
        </div>
      </div>

      <div class="right-col">
        <img class="hand-phone" src="/imgs/phoneBg-no-hand.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.bg {
  background: white url(/imgs/background-lines.svg);
}
.container {
  display: grid;
  justify-items: center;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  /*  padding-left: 210px; */

  border: 1px solid red;

  position: relative;
}

.hand-phone {
}

.page-head {
  .app-name {
    display: inline-block;
    background-color: $text-light-green;
    padding: 1rem 3rem;
    border-radius: 1rem 0 1rem 0;
    font-size: 1.5rem;
    color: #fff;
    font-weight: 500;
    margin-bottom: 2rem;
  }

  h1 {
    color: #1d1f22;
    font-family: Montserrat;
    font-size: 48px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;

    &:last-of-type {
      color: $text-light-green;
      margin-bottom: 3rem;
    }
  }

  p {
    font-size: 1.5rem;
    max-width: 520px;
  }
}

.description-container {
  .description-item {
    border-radius: 57px;
    background: #fff;
    box-shadow: 6px 6px 54px 0px rgba(0, 0, 0, 0.15);
    padding-left: 138px;
    /* TODO: FIX PADDING BOTTOM */
    padding: 16px 42px 3rem 138px;
    position: relative;
    max-width: 540px;
    font-weight: 500;
    margin-top: 110px;

    img {
      position: absolute;
      top: -150%;
      left: -5%;
    }

    &:last-of-type {
      margin-bottom: 85px;
    }
  }
}
</style>
