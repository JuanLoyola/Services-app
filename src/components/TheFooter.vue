<template>
  <div class="container">
    <h2 class="container-title">Lorem, ipsum dolor sit amet consectetur adipisicing.</h2>

    <div class="container-row">
      <a href="#" class="btnStarted">
        Get Started
      </a>
      <a href="#" class="btnLearn">
        Learn More
      </a>
    </div>
    <div class="container-row">
      <a class="footerMenu" href="#">Home</a>
      <a class="footerMenu" href="#">About</a>
      <a class="footerMenu" href="#">Services</a>
      <a class="footerMenu" href="#">FAQ</a>
    </div>

    <div class="container-row__social">
      <span class="icon">
        <a href="https://www.linkedin.com/in/loyolajuan/" target="_blank">
          <img class="iconIMG" src="@/assets/linkedin.svg" alt="linkedin logo">
        </a>
      </span>

      <span class="icon">
        <a href="https://github.com/JuanLoyola" target="_blank">
          <img class="iconIMG" src="@/assets/github.svg" alt="github logo">
        </a>
      </span>
    </div>

    <p class="copy"> &copy; 2021 Juan Loyola, all rights reserved.</p>
  </div>
</template>

<script>
export default {
  name: 'TheFooter'
}
</script>

<style lang="scss" scoped>
.container {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-flow: column nowrap;
  margin-top: 30px;

  &-title {
    font-size: 1.3rem;
  }

  &-row {
    width: 300px;
    display: flex;
    flex-flow: row wrap;
    justify-content: space-evenly;
    margin: 30px 0;

    .btnStarted {
      width: 110px;
      height: 41px;
      font-weight: 600;
      font-size: 0.8rem;
      line-height: 17px;
      display: flex;
      align-items: center;
      justify-content: center;
      letter-spacing: 0.05em;
      color: #FFFFFF;
      background-color: #4437B0;
      border-radius: 9px;
    }

    .btnLearn {
      width: 110px;
      height: 41px;
      font-weight: 600;
      font-size: 0.8rem;
      line-height: 17px;
      display: flex;
      align-items: center;
      justify-content: center;
      letter-spacing: 0.05em;
      color: #546BDC;
      background-color: #E5EDFF;
      border-radius: 9px;
    }

    .btnStarted:hover {
      background-color: #4337b0c0;
    }

    .btnLearn:hover {
      background-color: #d9dfeb;
    }

    .footerMenu {
      color: #989595;
    }
  }

  &-row__social {
    width: 100px;
    display: flex;
    flex-flow: row wrap;
    justify-content: space-evenly;
    margin: 20px 0;
  }
  .copy {
    color: #989595;
    margin-bottom: 30px;
  }
}
</style>
