<template>
  <div class="bg-color-white">
    <div class="container">
      <nav class="navbar navbar-expand-lg navbar-light ">
        <div class="container-fluid justify-content-between h-100">
          <a class="navbar-brand" href="#">
            <img src="../assets/img/dc-logo.png" alt="">
          </a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class=" collapse navbar-collapse flex-grow-0 h-100" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0 h-100">
              <li class=" nav-item h-100 " :class="{'ds-active' : link.isActive}" v-for="(link,index) in arrayHeaderLink" :key="`header-${index}`">
                <a class="nav-link-text d-flex align-items-center h-100" aria-current="page" :href="link.href">{{link.textLink}}</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
   </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderComp',
  data(){
    return {      
      arrayHeaderLink:[
        {
          href: '#',
          textLink: 'CHARACTERS',
          isActive: false
        },
        {
          href: '#',
          textLink: 'COMICS',
          isActive: true
        },
        {
          href: '#',
          textLink: 'TV',
          isActive: false
        },
        {
          href: '#',
          textLink: 'MOVIES',
          isActive: false
        },
        {
          href: '#',
          textLink: 'TV',
          isActive: false
        },
        {
          href: '#',
          textLink: 'GAMES',
          isActive: false
        },
        {
          href: '#',
          textLink: 'COLLECTIBLES',
          isActive: false
        },
        {
          href: '#',
          textLink: 'VIDEOS',
          isActive: false
        },
        {
          href: '#',
          textLink: 'FANS',
          isActive: false
        },
        {
          href: '#',
          textLink: 'NEWS',
          isActive: false
        },
        {
          href: '#',
          textLink: 'SHOP',
          isActive: false
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';

  .bg-color-white{
    background-color: white;
  }
  .nav-link-text{
    color: black;
    font-weight: bold;
    text-decoration: none;
    margin: 10px;
  }
  nav{
    height: 150px;
  }
  a{
    border-bottom: 4px solid transparent;
    cursor: pointer;
    background-color: red;
  }
  li.ds-active > a,
  li > a:hover {
    color: $primary-color;
    border-bottom: 14px solid $primary-color;
   
  }
</style>