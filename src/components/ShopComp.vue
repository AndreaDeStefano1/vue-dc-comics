<template>

  <div class="background-primary-light">

    <div class="container py-5 z-index">

      <ul class="d-flex align-items-center p-0 justify-content-between">
        <li v-for="(item,index) in ImageArr" :key="index" class="d-flex align-items-center"> 
          <img :src="require(`@/assets/img/${item.url}.${item.extension}`)" alt=""> 
          <a href="#">{{item.linkTitle}}</a> 
        </li>
      </ul>
    
    </div>

   
  </div>

</template>

<script>
export default {
  name: 'ShopComp',
  data(){
    return{
      ImageArr: [
        {
         linkTitle: 'DIGITAL COMICS',
          url: 'buy-comics-digital-comics',
          extension: 'png' 
        },
        {
         linkTitle: 'DC MERCHANDISE',
          url: 'buy-comics-merchandise',
          extension: 'png' 
        },
        {
         linkTitle: 'SUBSCRIPTION',
          url: 'buy-comics-subscriptions',
          extension: 'png' 
        },
        {
         linkTitle: 'COMIC SHOP LOCATOR',
          url: 'buy-comics-shop-locator',
          extension: 'png' 
        },
        {
          linkTitle: 'DC POWER VISA',
          url: 'buy-dc-power-visa',
          extension: 'svg'
        }
      ]
    }
  }
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