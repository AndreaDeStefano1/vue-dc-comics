<template>
  <div class="card card-w ">
    <div class="card no-bg">
      <div class="card-top overflow-hidden">
        <img :src="comic.thumb" class="card-img-top" alt="...">
      </div>
      
      <div class="card-body">
        <h6 class="card-title">{{comic.series}}</h6>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'CardComp',
  props:{
    comic: Object
  },
  
}
</script>

<style lang="scss" scoped>
  .card-w{
    width: calc(100% / 6);
    padding: 5px;
    
  }
  .card{
    background-color: transparent;
    border: none;
    color: white;
    text-transform: uppercase;
    
  }
  .no-bg{
    background-color: transparent;
  }
  .card-top{
    height: 200px;

  }
</style>