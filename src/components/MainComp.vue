<template>
  <div class="bg-color-black">

    <!-- in questo container stampo le carte -->
    <div class="container pb-3">

      <div class="card-container d-flex flex-wrap py-5 align-content-center h-100 position-relative">

        <div class="label-for-coimics position-absolute">
          <h3>CURRENT SERIES</h3>
        </div>
  
        <CardComp v-for='(comic,index) in comics' :key="`comic-${index}`" :comic="comic"/>
      </div>
      <div class=" m-auto w-mc">
        <button class="btn ds-btn"> LOAD MORE </button>

      </div>
      



    </div>

  </div>
</template>

<script>
import CardComp from './CardComp.vue';
import comicsData from '../assets/data/dc-comics.json'

export default {
    name: "MainComp",
    data(){
      return{
        comics: comicsData
      }
    },
    components: { 
      CardComp 
    }
}
</script>

<style lang='scss' scoped>
@import '../assets/style/vars';

.bg-color-black{
  background-color: #1c1c1c;

}
.label-for-coimics{
  top: -30px;
  z-index: 999;
  background-color: lighten($primary-color, 10%);
  color: white;
  padding: 5px 20px;
}
.ds-btn{
  background-color: lighten($primary-color, 10%);
  color: white;
  margin: 0 auto;
  padding: 5px 30px;
  font-weight: 700;
}
.w-mc{
  width: max-content;
}


</style>