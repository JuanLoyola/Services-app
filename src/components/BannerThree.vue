<template>
  <div class="container">
    <h2 class="container-title">Lorem ipsum dolor sit amet?</h2>

    <div class="row">
      <div class="column">

        <div class="item-row" data-aos="fade-right" data-aos-offset="400">
        <img class ="icon" src="@/assets/icon1.svg" alt="logo">
        <div class="content">
          <p class="content-title">1. Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet consectetur adipisicing.</p>
        </div>
      </div>

      <div class="item-row" data-aos="fade-right" data-aos-offset="400">
        <img class ="icon" src="@/assets/icon2.svg" alt="logo">
        <div class="content">
          <p class="content-title">2. Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet consectetur adipisicing.</p>
        </div>
      </div>

      <div class="item-row" data-aos="fade-right" data-aos-offset="400">
        <img class ="icon" src="@/assets/icon3.svg" alt="logo">
        <div class="content">
          <p class="content-title">3. Lorem, ipsum.</p>
          <p class="content-info">Lorem ipsum dolor, sit amet consectetur adipisicing.</p>
        </div>
      </div>
      </div>

      <div class="background">
        <img class="example" data-aos="fade-left" src="@/assets/exampleImg.svg" alt="example">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BannerThree'
}
</script>

<style lang="scss" scoped>
.container {
  width: 100%;
  height: 631px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-flow: column nowrap;

  &-title {
    font-size: 2rem;
    text-align: center;
  }

  .row {
    width: 100%;
    display: flex;
    justify-content: space-evenly;
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

@media (min-width: 320px) and (max-width: 1023px) {
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
      flex-flow: column nowrap;

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
@media (min-width: 320px) and (max-width: 1024px) {
    .container {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-flow: column nowrap;
    &-title {
      font-size: 1.3rem;
      margin-top: 30px;
    }

    .row {
      flex-flow: row wrap;

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
