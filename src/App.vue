<template>
  <div>
   <HeaderComp/>

   <MainComp/>

   <ShopComp/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import ShopComp from './components/ShopComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    ShopComp
    
  }
}
</script>

<style lang="scss">

</style>
