<template>
  <nav class="nav nav__fixed nav__fixed-top">
    <ul class="nav__list">
      <li class="nav__item">
        <nuxt-link to="/">Curratelo.es</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/realtime">Realtime</nuxt-link>
      </li>
    </ul>
  </nav>
</template>

<style lang="scss" scoped>
  @import '@/assets/styles/config.scss';
  
  .nav {
    color: red;
    background-color: $primary;
    color: rgba(255,255,255,.84);
    width: 100%;
    height: 4rem;  
    display: flex;

    &__fixed{
      position: fixed;
      z-index: 1;
      &-top{
        top:0;
        left: 0;
      }
    }
    &__item{
      color: blue
    }

    @include media(md){
      
    }
    
    &__list{
      max-width: $maxWidth;
      display:flex;
      flex-flow:row nowrap;
      justify-content: space-around;
      
    }
  }
</style>
