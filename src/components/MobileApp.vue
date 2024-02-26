<template>
  <div class="bg">
    <div class="container">
      <div class="left-col">
        <div class="page-head">
          <p class="app-name">Mobile App</p>

          <!--  <h1>Lorem, ipsum dolor.</h1> -->
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
        <img class="phone" src="/imgs/phoneBg-no-hand.png" alt="" />
        <div class="links-stats-wrapper">
          <div class="links">
            <a href="#"
              ><img src="/imgs/apple-logo.png" alt="apple-logo" href="#"
            /></a>
            <a href="#">
              <img
                src="/imgs/playmarket-logo.png"
                alt="playmarket-logo"
                href="#"
              />
            </a>
            <a href="#"><img src="/imgs/rustore.png" alt="ruStore-logo" /></a>
          </div>
          <div class="subsidy-wrapper">
            <img class="subsidy-stats" src="/imgs/subsidy-stats.svg" alt="" />
          </div>
        </div>
        <img class="smev" src="/imgs/smev.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.bg {
  padding: 2rem 0;
  background: white url(/imgs/background-lines.svg);
}
.container {
  display: flex;
  flex-direction: row;

  justify-items: center;
  align-items: center;
  flex-wrap: wrap;

  /*  padding-left: 210px; */

  position: relative;
}

.left-col {
  margin-left: 10%;
}

.right-col {
  display: flex;
  /* padding-left: 3rem; */
  justify-content: flex-start;
  position: relative;

  .phone {
    width: 100%;
    z-index: 10;
  }
  .smev {
    position: absolute;
    z-index: 0;
    bottom: -10%;
    left: -10%;
  }

  /*  @media () */
}

.links-stats-wrapper {
  z-index: 5;
  margin-left: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  .links {
    display: flex;
    width: 100%;
    align-items: center;
    justify-content: space-between;
    img {
      padding: 18px;

      border-radius: 23px;
      background: #fff;
      box-shadow: 6px 6px 24px 0px rgba(0, 0, 0, 0.1);

      transition: 0.5s;
      &:hover {
        transform: translateY(-10px);
      }
    }
  }

  .subsidy-wrapper {
    margin-top: 22px;
    width: fit-content;

    img {
      border-radius: 14px;
      background: #fff;
      box-shadow: 6px 6px 54px 5px rgba(0, 0, 0, 0.2);
    }
  }
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

    transition: 0.5s;
    &:hover {
      transform: translateY(-10px);
    }

    img {
      position: absolute;
      top: -150%;
      left: -5%;

      @media screen and (max-width: 580px) {
        top: -115%;
      }
    }

    &:last-of-type {
      margin-bottom: 2rem;
    }
  }
  .navigation-item {
    margin-bottom: 2rem;
  }
}

@media screen and (max-width: 1600px) {
  .links-stats-wrapper {
    margin-left: 0.25rem;
  }
  @media screen and (min-width: 1072px) and (max-width: 1560px) {
    .right-col {
      flex-direction: column;
    }
    .links-stats-wrapper {
      flex-direction: column-reverse;
    }
  }
}

@media screen and (min-width: 1072px) {
  .right-col {
    margin-top: 2rem;
    width: 30%;
  }
}

@media screen and (max-width: 962px) {
  .right-col {
    width: 60%;
  }
}
@media screen and (max-width: 758px) {
  .right-col {
    width: 50%;
  }
}
@media screen and (max-width: 600px) {
  .left-col {
    padding: 0 0.5rem;
    margin: 0 auto;
  }
  .right-col {
    margin: 0 auto;
    width: 70%;
    flex-direction: column;
  }
  .links-stats-wrapper {
    flex-direction: column-reverse;
  }
}
</style>
