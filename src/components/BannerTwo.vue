<template>
  <div class="container">
    <h2 class="container__title">
      Lorem, ipsum dolor.
    </h2>
    <h4 class="container__subtitle">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Laudantium dolor qui magnam facilis quasi! Sed <br> magni nesciunt quod.
    </h4>
    <div class="row">
      <div class="item-row" data-aos="fade-down">
        <img class ="icon" src="@/assets/icon1.svg" alt="logo">
        <div class="content">
          <p class="content-title">Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet <br> consectetur adipisicing.</p>
        </div>
      </div>

      <div class="item-row" data-aos="fade-down">
        <img class ="icon" src="@/assets/icon2.svg" alt="logo">
        <div class="content">
          <p class="content-title">Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet <br> consectetur adipisicing.</p>
        </div>
      </div>

      <div class="item-row" data-aos="fade-down">
        <img class ="icon" src="@/assets/icon3.svg" alt="logo">
        <div class="content">
          <p class="content-title">Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet <br> consectetur adipisicing.</p>
        </div>
      </div>

      <div class="item-row" data-aos="fade-down">
        <img class ="icon" src="@/assets/icon4.svg" alt="logo">
        <div class="content">
          <p class="content-title">Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet <br> consectetur adipisicing.</p>
        </div>
      </div>

      <div class="item-row" data-aos="fade-down">
        <img class ="icon" src="@/assets/icon5.svg" alt="logo">
        <div class="content">
          <p class="content-title">Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet <br> consectetur adipisicing.</p>
        </div>
      </div>

      <div class="item-row" data-aos="fade-down">
        <img class ="icon" src="@/assets/icon6.svg" alt="logo">
        <div class="content">
          <p class="content-title">Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet <br> consectetur adipisicing.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BannerTwo'
}
</script>

<style lang="scss" scoped>
.container{
  width: 100%;
  height: 517px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-flow: column nowrap;
  background-color: #f7f4f4;

  &__title {
    width: 50%;
    font-weight: bold;
    font-size: 3.5rem;
    line-height: 59px;
    letter-spacing: 2px;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;

    color: #333333;
    margin-top: 20px;
    margin-bottom: 18px;
  }

  &__subtitle {
    font-weight: 500;
    line-height: 21px;

    color: #76828A;
    margin-bottom: 10px;
  }

  .row {
    width: 60%;
    height: 338px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-flow: row wrap;

    .item-row {
      display: flex;
      flex-direction: row;

      .content {
        display: flex;
        flex-direction: column;
        text-align: start;
        margin-left: 10px;
        line-height: 20px;

        &-title {
          font-weight: 700;
          font-size: 1.4rem;
          margin-bottom: 10px;
        }

        &-info {
          font-weight: 500;
        }
      }
    }
  }
}

@media (min-width: 320px) and (max-width: 1024px) {
  .container{
  height: 100%;
  &__title {
    width: 100%;
    font-size: 1.5rem;
    line-height: 30px;
    margin-top: 40px;
  }

  &__subtitle {
    font-weight: 500;
    line-height: 21px;

    color: #76828A;
    margin-bottom: 30px;
  }

  .row {
    height: 100%;
    width: 100%;

    .item-row {
      margin-bottom: 30px;

      .content {
        display: flex;
        flex-direction: column;
        text-align: start;
        margin-left: 10px;
        line-height: 20px;

        &-title {
          font-weight: 700;
          font-size: 1.4rem;
          margin-bottom: 10px;
        }

        &-info {
          font-weight: 500;
        }
      }
    }
  }
}
}
</style>
