<template>
  <div class="container">

    <div class="container-status">
      <div class="type"><span>{{ status }}</span></div>
      <div class="priceType">
        <span class="price">${{ price }}</span><p class="time">/mo</p>
      </div>
    </div>

    <div class="content">
      <div class="content-row">
        <span><i class="icon fas fa-check"></i></span><p>Lorem ipsum.</p>
      </div>
      <div class="content-row">
        <span><i class="icon fas fa-check"></i></span><p>Lorem ipsum.</p>
      </div>
      <div class="content-row">
        <span><i class="icon fas fa-check"></i></span><p>Lorem ipsum.</p>
      </div>
      <div class="content-row">
        <span><i class="icon fas fa-check"></i></span><p>Lorem ipsum.</p>
      </div>
      <div class="content-row">
        <span><i class="icon fas fa-check"></i></span><p>Lorem ipsum.</p>
      </div>
      <div class="content-row">
        <span><i class="icon fas fa-check"></i></span><p>Lorem ipsum.</p>
      </div>
    </div>

    <div class="btn">
      <p>Get started</p>
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
  margin: 0 10px;
  cursor: pointer;

  &-status {
    background: #ffffff;
    width: 257px;
    height: 120px;
    border-radius: 10px;

    display: flex;
    flex-flow: column nowrap;

    .type {
      width: 102px;
      height: 30px;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #E5EDFF;
      color: #686FF1;
      font-weight: 600;
      text-transform: uppercase;
      border-radius: 9px;
      margin: 18px 0 18px 16px;
    }

    .priceType {
      display: flex;
      flex-flow: row nowrap;
      justify-content: center;
      align-items: flex-end;
      margin: 0 20px;

      .price {
        font-size: 3rem;
        font-weight: 600;
      }

      .time {
        font-weight: 500;
        font-size: 1.3rem;
      }
    }
  }

  .content{
    display: flex;
    flex-flow: column nowrap;
    align-items: center;
    justify-content: center;
    margin: 18px 0;

    &-row {
      width: 70%;
      display: flex;
      flex-flow: row nowrap;
      justify-content: space-evenly;
      color: #A59A98;
      margin: 10px 0;

      .icon {
        color: #5AC174;
      }
    }
  }

  .btn {
    width: 197px;
    height: 40px;
    border-radius: 9px;
    background:  #000;
    color: #ffffff;
    font-weight: 500;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0px 30px 18px 30px;
  }
}
</style>
