<template>
  <div class="background-primary-light">
    <div class="container py-5 z-index">

      <ul class="d-flex align-items-center p-0 justify-content-between">

        <li class="d-flex align-items-center">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <a href="#">DIGITAL COMICS</a>
        </li>

        <li class="d-flex align-items-center">       
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          <a href="#">DC MERCHANDISE</a> 
        </li>

        <li class="d-flex align-items-center">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <a href="#">SUBSCRIPTION</a> 
        </li>

        <li class="d-flex align-items-center">
          <img class="shop-locator" src="../assets/img/buy-comics-shop-locator.png" alt="">
          <a href="#">COMIC SHOP LOCATOR</a> 
        </li>

        <li class="d-flex align-items-center"> 
          <img src="../assets/img/buy-dc-power-visa.svg" alt=""> 
          <a href="#">DC POWER VISA</a> 
        </li>
        
        
      </ul>
    
    </div>

   
  </div>
</template>

<script>
export default {
  name: 'ShopComp'
}
</script>

<style lang='scss' scoped>

  @import '../assets/style/vars';

  .background-primary-light{
    background-color: lighten($primary-color, 10%);
    
  }
  ul{
    list-style: none;
  }

  img{
    transform: scale(0.5);

    
  }
  li{
    a{
      color: white;
      text-decoration: none;
      white-space: nowrap
    }
  }

</style>