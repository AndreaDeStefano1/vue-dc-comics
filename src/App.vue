<template>
  <div>

   <HeaderComp/>

   <JumbotronComp/>

   <MainComp/>

   <ShopComp/>

  <FooterComp/>


  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import ShopComp from './components/ShopComp.vue'
import FooterComp from './components/FooterComp.vue'
import JumbotronComp from './components/JumbotronComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    ShopComp,
    FooterComp,
    JumbotronComp
}
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
