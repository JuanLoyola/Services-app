<template>
  <div class="container">

    <div class="row">
      <div class="background">
        <img class="example" src="@/assets/exampleImg.svg" alt="example">
      </div>
      <div class="column">

        <div class="item-row">
        <img class ="icon" src="@/assets/icon4.svg" alt="logo">
        <div class="content">
          <p class="content-title">4. Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet consectetur adipisicing.</p>
        </div>
      </div>

      <div class="item-row">
        <img class ="icon" src="@/assets/icon5.svg" alt="logo">
        <div class="content">
          <p class="content-title">5. Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet consectetur adipisicing.</p>
        </div>
      </div>

      <div class="item-row">
        <img class ="icon" src="@/assets/icon6.svg" alt="logo">
        <div class="content">
          <p class="content-title">6. Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet consectetur adipisicing.</p>
        </div>
      </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'BannerFour'
}
</script>

<style lang="scss" scoped>
.container {
  width: 100%;
  height: 631px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: -50px;
  &-title {
    font-size: 2rem;
    text-align: center;
  }

  .row {
    width: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-flow: row nowrap;
    margin-top: 40px;

    .column {
      width: 30%;
      text-align: start;

      .title {
        font-size: 1.5rem;
        font-weight: 600;
        margin-bottom: 20px;
      }

      .info {
        width: 70%;
        color: #76828A;
        font-weight: 500;
        margin-bottom: 20px;
      }

      .item-row {
        display: flex;
        flex-direction: row;
        margin-bottom: 10px;

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

        .icon {
          width: 55px;
          height: 55px;
        }
      }
    }
  }
}

@media (min-width: 320px) and (max-width: 1024px) {
    .container {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-flow: column nowrap;
    &-title {
      font-size: 1.3rem;
    }

    .row {
      flex-flow: column-reverse nowrap;

      .column {
        width: 100%;
        text-align: center;

        .info {
          width: 100%;
        }

        .item-row {
          justify-content: center;
        }
      }

      .background {
        background-image: none;

        .example {
          width: 320px;
        }
      }
    }
  }
}
</style>
