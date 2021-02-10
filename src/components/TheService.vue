<template>
  <div class="container">
    <div class="background">

      <div class="column" data-aos="flip-up">
        <blockquote class="column__info"> <span class="quote">"</span>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sint quam quo ipsam eaque vel, illum earum minima quisquam modi sit, voluptatum fuga doloribus quae nam.
        </blockquote>
        <div class="column__sign">
          <img class="avatar" src="@/assets/user.png" alt="Avatar Image">
          <div class="user">
            <p class="user__name">Garfield Lorem</p>
            <p class="user__info">CEO, Lorem CO</p>
          </div>
        </div>
      </div>

      <div class="separator">
        <div class="line"></div>
      </div>

      <div class="column" data-aos="flip-up">
        <blockquote class="column__info"> <span class="quote">"</span>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sint quam quo ipsam eaque vel, illum earum minima quisquam modi sit, voluptatum fuga doloribus quae nam.
        </blockquote>
        <div class="column__sign">
          <img class="avatar" src="@/assets/user.png" alt="Avatar Image">
          <div class="user">
            <p class="user__name">Garfield Lorem</p>
            <p class="user__info">CEO, Lorem CO</p>
          </div>
        </div>
      </div>

      <div class="info">
        <div class="content">
        <h2 class="title">Lorem ipsum dolor sit amet.</h2>
        <h4 class="subtitle">Lorem ipsum dolor sit.</h4>
      </div>

      <div class="cards"
      >
        <TheCard
        status="started"
        price="3"
        ></TheCard>

        <TheCard
        status="advance"
        price="10"
        ></TheCard>

        <TheCard
        status="pro"
        price="49"
        ></TheCard>
      </div>

      </div>
    </div>
  </div>
</template>

<script>
import TheCard from '@/components/TheCard.vue'

export default {
  name: 'TheService',

  components: {
    TheCard
  }
}
</script>

<style lang="scss" scoped>
.container {
  width: 100%;
  height: 1154px;

  .background {
    width: 100%;
    height: 812px;
    background-color: #17123B;
    display: flex;
    justify-content: space-around;
    flex-flow: row wrap;

    .column {
      width: 570px;
      height: 200px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: start;
      margin-top: 52px;

      &__info {
        font-weight: 500;
        font-size: 1.3rem;
        line-height: 20px;
        display: flex;
        align-items: center;
        color: #FFFFFF;
        margin-bottom: 12px;

        .quote {
          font-size: 4rem;
          font-family:'Times New Roman', Times, serif;
          display: flex;
          align-self: flex-start;
          color: #A9CFF7;
        }
      }

      &__sign {
        display: flex;
        flex-flow: row nowrap;
        width: 100%;

        .avatar {
          width: 68px;
          height: 62px;
          border-radius: 50%;
          margin-right: 22px;
          border: 2px solid #ffffff;
        }

        .user {
          display: flex;
          flex-flow: column nowrap;

          &__name {
            font-weight: 500;
            font-size: 1.2rem;
            line-height: 18px;
            display: flex;
            align-items: center;
            color: #FFFFFF;
            margin-bottom: 12px;
          }

          &__info {
            font-size: 0.8rem;
            font-weight: bold;
            line-height: 12px;
            display: flex;
            align-items: center;
            color: #A9CFF7;
          }
        }
      }
    }

    .separator {
      height: 261px;
      display: flex;
      align-items: center;
      .line {
        width: 262px;
        height: 0px;
        border: 2px solid #4A419F;
        box-shadow: 0px 0px 11px rgba(255, 255, 255, 0.25);
        transform: rotate(90deg);
      }
    }

    .info {
      display: flex;
      flex-flow: column nowrap;
      .content {
        .title {
          font-size: 3rem;
          color: #ffffff;
        }

        .subtitle {
          font-size: 1.3rem;
          color: #83808F;
          margin-top: 10px;
          margin-bottom: 30px;
        }
      }
      .cards {
        display: flex;
        justify-content: center;
        flex-flow: row nowrap;
        width: 771px;
        height: 454px;
        margin-top: 70px;
      }
    }
  }
}

@media (min-width: 320px) and (max-width: 1023px){
  .container {
    width: 100%;
    height: 100%;

    .background {
      width: 100%;
      height: 100%;

      .column {
        &__info {
          font-size: 1rem;

          .quote {
            font-size: 2rem;
          }
        }

        &__sign {

          .avatar {
            width: 58px;
            height: 52px;
          }

          .user {
            display: flex;
            flex-flow: column nowrap;

            &__name {
              font-weight: 500;
              font-size: 1rem;
              line-height: 18px;
              display: flex;
              align-items: center;
              color: #FFFFFF;
              margin-bottom: 12px;
            }

            &__info {
              font-size: 0.7rem;
              font-weight: bold;
              line-height: 12px;
              display: flex;
              align-items: center;
              color: #A9CFF7;
            }
          }
        }
      }

      .separator {
        .line {
          transform: rotate(0deg);
        }
      }

      .info {
        .content {
          .title {
            font-size: 2rem;
            margin-top: 30px;
          }
        }
        .cards {
          flex-flow: column nowrap;
          justify-content: center;
          align-self: center;
          width: 271px;
          height: 100%;
          margin-top: 20px;
        }
      }
    }
  }
}

@media (min-width: 1024px) and (max-width: 1366px){
  .container {
    width: 100%;
    height: 100%;

    .background {
      width: 100%;
      height: 100%;
      display: flex;
      flex-flow: row wrap;
      justify-content: center;
      align-items: center;

      .column {
        max-width: 350px;
        &__info {
          font-size: 1rem;

          .quote {
            font-size: 2rem;
          }
        }

        &__sign {

          .avatar {
            width: 58px;
            height: 52px;
          }

          .user {
            display: flex;
            flex-flow: column nowrap;

            &__name {
              font-weight: 500;
              font-size: 1rem;
              line-height: 18px;
              display: flex;
              align-items: center;
              color: #FFFFFF;
              margin-bottom: 12px;
            }

            &__info {
              font-size: 0.7rem;
              font-weight: bold;
              line-height: 12px;
              display: flex;
              align-items: center;
              color: #A9CFF7;
            }
          }
        }
      }

      .separator {
        .line {
          transform: rotate(90deg);
        }
      }

      .info {
        .content {
          .title {
            font-size: 2rem;
            margin-top: 30px;
          }
        }
        .cards {
          flex-flow: row nowrap;
          justify-content: center;
          align-self: center;
          width: 271px;
          height: 100%;
          margin-top: 30px;
          margin-bottom: 30px;
        }
      }
    }
  }
}

</style>
