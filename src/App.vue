<template>
  <div>

   <HeaderComp/>

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

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    ShopComp,
    FooterComp
}
}
</script>

<style lang="scss">

</style>
