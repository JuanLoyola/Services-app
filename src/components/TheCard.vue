<template>
  <div class="container">
    <div class="container-status">
      <div class="type"><span>{{ status }}</span></div>
      <div class="priceType">
        <span class="price">${{ price }}</span><p class="time">/mo</p>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'TheCard',

  props: {
    status: {
      type: String,
      required: true
    },

    price: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.container {
  width: 257px;
  max-height: 454px;
  background-color: #F9FAFB;
  border-radius: 10px;
  box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.25);

  &-status {
    background: #ffffff;
    width: 257px;
    height: 120px;
    border-radius: 10px;

    display: flex;
    flex-flow: column nowrap;
    justify-content: flex-start;
    align-items: flex-start;

    .type {
      width: 102px;
      height: 30px;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #E5EDFF;
      color: #686FF1;
      font-weight: 500;
      text-transform: uppercase;
      border-radius: 9px;
      margin: 18px 0 18px 16px;
    }

    .priceType {
      display: flex;
      flex-flow: row nowrap;
      justify-content: center;
      align-items: center;
      margin: 0 20px;

      .price {
        font-size: 2.3rem;
        font-weight: 600;
      }

      .time {
        font-weight: 500;
        font-size: 1rem;
      }
    }
  }
}
</style>
