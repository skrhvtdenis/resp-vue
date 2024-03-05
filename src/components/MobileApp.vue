<template>
  <div class="bg">
    <section class="container">
      <div class="info-col">
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

      <div class="phone-col">
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
    </section>

    <section class="respak-page">
      <section class="container">
        <div class="vidgets-col">
          <img src="/imgs/vidgets-page.png" draggable="false" alt="" />
        </div>
        <div class="info-col">
          <div class="page-head">
            <p class="app-name">WEB-System</p>

            <h1>Lorem, ipsum dolor.</h1>
            <h1>СИСТЕМА ИС.РЕСПАК</h1>

            <p>
              Решение для сельского хозяйства, обеспечивающее цифровое
              взаимодействие органов власти и сельхозтоваропроизводителей
              региона.
            </p>
          </div>
          <div class="grid-container">
            <div class="grid-item">
              <img src="/imgs/database.svg" alt="" />
              <h4>Разработка</h4>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmodadipiscing elit, sed do eiusmod
              </p>
              <a href="#">
                <div class="btn-holder">
                  <img src="/imgs/small-arrow.svg" alt="" />
                </div>
              </a>
            </div>
            <div class="grid-item">
              <img src="/imgs/soprovod.svg" alt="" />
              <h4>Сопровождение</h4>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmodadipiscing elit, sed do eiusmod
              </p>
              <a href="#">
                <div class="btn-holder">
                  <img src="/imgs/small-arrow.svg" alt="" />
                </div>
              </a>
            </div>
            <div class="grid-item">
              <img src="/imgs/analytics.svg" alt="" />
              <h4>Аналитика</h4>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmodadipiscing elit, sed do eiusmod
              </p>
              <a href="#">
                <div class="btn-holder">
                  <img src="/imgs/small-arrow.svg" alt="" />
                </div>
              </a>
            </div>
            <div class="grid-item">
              <img src="/imgs/monitor.svg" alt="" />
              <h4>Something</h4>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmodadipiscing elit, sed do eiusmod
              </p>
              <a href="#">
                <div class="btn-holder">
                  <img src="/imgs/small-arrow.svg" alt="" />
                </div>
              </a>
            </div>

            <p class="navigation-item">
              <a href="#" class=""
                >все проекты <img src="/imgs/arrow.png" alt=""
              /></a>
            </p>
          </div>
        </div>
      </section>
    </section>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.bg {
  padding: 2rem 0;
  background: white url(/imgs/background-lines.png);
  background-size: cover;
}
.container {
  display: flex;
  flex-direction: row;

  justify-items: center;
  align-items: center;
  flex-wrap: wrap;

  /*  padding-left: 210px; */

  position: relative;
  margin-bottom: 6rem;
}

.info-col {
  margin-left: 10%;
}

.phone-col {
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
  justify-content: flex-start;
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
    font-size: 3rem;
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
    font-weight: 500;
    color: #1d1f22;
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

/* SECOND PAGE STYLES */

.respak-page {
  .vidgets-col {
    align-self: flex-end;
  }

  .info-col {
    margin-left: 0;
  }

  .grid-container {
    margin-top: 3em;
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr;
    font-size: 1rem;
    gap: 3em 5em;
  }

  .grid-item {
    background-color: #ffffff;
    max-width: 270px;
    border-radius: 20px;
    box-shadow: 0px 18.829999923706055px 47.08000183105469px 0px #2f327d1a;
    display: flex;
    padding: 1em 1.5em;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    transition: background-color 1s;
    font-size: 1rem;

    h4 {
      font-size: 1.25rem;
      font-weight: 700;
      margin-top: 1rem;
      margin-bottom: 1rem;
    }

    p {
      font-size: 14px;
      text-align: center;
      margin-bottom: 0.5rem;
    }
    a {
      align-self: flex-end;
    }
    .btn-holder {
      display: flex;
      opacity: 0;
    }

    &:hover {
      background-color: #1d1f22;

      color: #ffffff;

      h4 {
        text-decoration: underline;
      }

      .btn-holder {
        opacity: 100%;
      }
    }
  }
}

.vidgets-col {
  width: 60%;
  img {
    width: 100%;
  }
}

/* FIRST PAGE MEDIA QUERIES */
@media screen and (max-width: 1600px) {
  .links-stats-wrapper {
    margin-left: 0.25rem;
  }
  @media screen and (min-width: 1072px) and (max-width: 1560px) {
    .phone-col {
      flex-direction: column;
    }
    .links-stats-wrapper {
      flex-direction: column-reverse;
    }
  }
}

@media screen and (min-width: 1072px) {
  .phone-col {
    margin-top: 2rem;
    width: 30%;
  }
}

@media screen and (max-width: 962px) {
  .phone-col {
    width: 60%;
  }
}
@media screen and (max-width: 758px) {
  .phone-col {
    width: 50%;
  }
}
@media screen and (max-width: 600px) {
  .info-col {
    padding: 0 0.5rem;
    margin: 0 auto;
  }
  .phone-col {
    margin: 0 auto;
    width: 70%;
    flex-direction: column;
  }
  .links-stats-wrapper {
    flex-direction: column-reverse;
  }
  .smev {
    width: 100%;
  }

  .page-head {
    h1 {
      font-size: 2rem;
    }
    p {
      font-size: 1.25rem;
    }
  }
}

/* RESPAK PAGE MEDIA QUERIES */

@media screen and (max-width: 768px) {
  .grid-container {
    font-size: 8px !important;
  }
}
</style>
