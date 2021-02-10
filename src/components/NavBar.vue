<template>
  <div id="nav">
      <div>
        <input type="checkbox" id="click">
      <label for="click" class="menu-btn">
        <i class="fas fa-bars"></i>
      </label>
      <ul class="menu">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">FAQ</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style lang="scss">
#nav {
  display: flex;
  height: 126px;
  width: 100%;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  z-index: 2;

  font-family: 'Montserrat';
  color: #76828A;
  background: #17123B;

  .logo {
    margin-left: 100px;
    width: 40px;
    height: 58px;
  }
}
#nav ul{
    display: flex;
    flex-wrap: wrap;
    list-style: none;
  }
  #nav ul li{
    margin: 0 2px;
  }
  #nav ul li a{
    color: #88949c;
    text-decoration: none;
    font-size: 1rem;
    font-weight: 500;
    padding: 8px 1rem;
    border-radius: 5px;
    letter-spacing: 1px;
    transition: all 0.3s ease;
  }
  #nav ul li a:hover{
    color:#F27373;
  }
  #nav .menu-btn i{
    color: #fff;
    font-size: 22px;
    padding: 0 30px;
    cursor: pointer;
    display: none;
  }

  input[type="checkbox"] {
    display: none;
  }
  @media (max-width: 1000px){
    #nav{
      height: 88px;
      padding: 0 40px 0 50px;
    }
  }
  @media (max-width: 920px) {
    #nav .menu-btn i{
      display: block;
    }
    #click:checked ~ .menu-btn i:before{
      content: "\f00d";
    }
    #nav ul{
      position: fixed;
      top: 80px;
      left: -100%;
      background: #111;
      height: 100vh;
      width: 100%;
      text-align: center;
      display: block;
      transition: all 0.3s ease;
    }
    #click:checked ~ ul{
      left: 0;
    }
    #nav ul li{
      width: 100%;
      margin: 40px 0;
    }
    #nav ul li a{
      width: 100%;
      margin-left: -100%;
      display: block;
      font-size: 20px;
      transition: 0.6s cubic-bezier(0.68, -0.55, 0.265, 1.55);
    }
    #click:checked ~ ul li a{
      margin-left: 0px;
    }
    #nav ul li a.active,
    #nav ul li a:hover{
      background: none;
      color: #F27373;
    }
  }
  @media screen and (min-width: 320px) and (max-width:1034px){
    #nav{
      padding: 0px 0px;
      display:flex;
      width:100%;

      .name{
        font-size: 0.8rem;
      }

      a{
        font-size: 0.6rem;
        display:flex;
        flex-direction: row wrap;
      }
    }
  }
</style>
