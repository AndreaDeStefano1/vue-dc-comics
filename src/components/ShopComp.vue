<template>
  <div class="background-primary-light">
    <div class="container py-5">

      <ul class="d-flex align-items-center justify-content-between">

        <li>
          <div class="image">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          </div>
          <div class="category-name">
            <a href="#">Digital Comics</a> 
          </div>
        </li>

        <li>
          <div class="image">
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
          </div>
          <div class="category-name">
            <a href="#">DC MERCHANDISE</a> 
          </div>
        </li>

        <li>
          <div class="image">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
          </div>
          <div class="category-name">
            <a href="#">SUBSCRIPTION</a> 
          </div>
        </li>

        <li>
          <div class="image">
            <img class="shop-locator" src="../assets/img/buy-comics-shop-locator.png" alt="">
          </div>
          <div class="category-name">
            <a href="#">COMIC SHOP LOCATOR</a> 
          </div>
        </li>

        <li>
          <div class="image">
            <!-- Non funziona-->
            <img src="../assets/img/buy-dc-power-visa.svg" alt=""> 
          </div>
          <div class="category-name">
            <a href="#">DC POWER VISA</a> 
          </div>
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
  li > div{
    display: inline-block;
  }
  img{
    transform: scale(0.5);

    
  }

  li a{
    color: white;
    text-decoration: none;
  }

</style>