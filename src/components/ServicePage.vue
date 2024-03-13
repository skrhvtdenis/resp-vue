<template>
  <div>
    <section class="respak-services">
      <div class="info-col">
        <h2>Сервисы ИС.РЕСПАК</h2>
        <div class="grid-container">
          <div class="grid-header">
            <p>Система переведена на ГосТех</p>
            <img src="/imgs/gosteh.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Субсидии</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Земельный паспорт</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Интеграции с прочими системами</p>
            <img src="/imgs/integration.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Отчетность</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>BI-Аналитика</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Цифровой профиль</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Гранты</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Вход через ЕСИА</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Реестр СХП</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Агрометео сервис</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Соглашения</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
          <div class="grid-item">
            <p>Межведы</p>
            <img src="/imgs/vidget-dashboard.svg" alt="" />
          </div>
        </div>

        <p class="navigation-item">
          <a href="#" class=""
            >Смотреть все <img src="/imgs/arrow.png" alt=""
          /></a>
        </p>
      </div>
      <div class="img-col">
        <!--      <img src="/imgs/thumbs-up.png" alt="" /> -->
      </div>
    </section>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.respak-service {
  display: flex;
  flex-direction: row;
}

.info-col {
  display: flex;
  flex-direction: column;
  align-items: center;
  h2 {
    font-size: 3rem;
    font-style: bold;
    text-align: center;
  }

  .grid-container {
    display: grid;
    grid-template-columns: repeat(3, minmax(120px, 150px));

    gap: 3rem;

    /*  @media screen and (max-width: 600px) {
      grid-template-columns: repeat(2, minmax(120px, 150px));
      gap: 2rem;
    }
    @media screen and (max-width: 500px) {
      grid-template-columns: repeat(2, minmax(120px, 150px));
      gap: 1.5rem;
    } */
  }

  .grid-header {
    background-color: #fff;
    grid-column-start: span 3;
    border-radius: 20px;
    box-shadow: 6px 6px 24px 0px rgba(0, 0, 0, 0.1);
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2rem 4rem;
    p {
      text-align: center;
      margin-bottom: 1.25rem;
    }
    img {
      width: 100%;
    }
  }
  .grid-item {
    background-color: #fff;
    padding-top: 1rem;

    border-radius: 20px;
    box-shadow: 6px 6px 24px 0px rgba(0, 0, 0, 0.1);
    display: flex;
    flex-direction: column;
    justify-content: space-between;

    p {
      padding-inline: 1rem;
      font-size: 14px;
      font-weight: 500;
      text-align: center;
    }

    img {
      width: 80px;
    }
  }
}

@media screen and (max-width: 600px) {
  .info-col .grid-container {
    grid-template-columns: repeat(2, minmax(120px, 150px));
    gap: 2rem;
  }
  .info-col .grid-header {
    grid-column-start: span 2;
  }
}
@media screen and (max-width: 500px) {
  .info-col .grid-container {
    gap: 1.5rem;
  }
  .info-col .grid-header {
    grid-column-start: span 2;
  }
}
</style>
