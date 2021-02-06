<template>
  <div class="container">
    <h2 class="container__title">
      Lorem ipsum dolor sit amet & consectetur adipisicing.
    </h2>
    <h4 class="container__subtitle">
      Lorem ipsum dolor, sit amet consectetur adipisicing elit.
      <br>Magni expedita velit earum?
    </h4>
    <a href="#" target="_blank" class="btn">Start your free 7-day trial</a>
  </div>
</template>

<script>
export default {
  name: 'BannerOne'
}
</script>

<style lang="scss" scoped>
.container{
  width: 100%;
  height: 413px;
  background: #17123B;
  display: flex;
  align-items: center;
  flex-flow: column nowrap;

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

    color: #FFFFFF;

    text-shadow: -4px 4px 25px #8E81F7;
    margin-top: 30px;
    margin-bottom: 30px;
  }

  &__subtitle {
    font-weight: 500;
    line-height: 21px;

    color: #76828A;
    margin-bottom: 40px;
  }

  .btn {
    width: 234px;
    height: 42px;
    background-color: #4437B0;
    color: #ffffff;
    text-decoration: none;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 9px;
  }
}

@media (min-width: 320px) and (max-width: 1366px) {
  .container {
    &__title {
      font-size: 2rem;
      line-height: 30px;
      text-align: center;
    }
  }
}
</style>
