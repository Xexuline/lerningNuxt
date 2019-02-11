<template>
  <nav class="nav__fixed nav__fixed-top">
    <ul class="nav">
      <li class="nav__item">
        <nuxt-link to="/">Curratelo.es</nuxt-link>
      </li>
      <li class="nav__item">
        <nuxt-link to="/realtime">Realtime</nuxt-link>
      </li>
    </ul>
  </nav>
</template>

<style lang="scss" scoped>
  @import '@/assets/styles/config.scss';
  
  .nav {
    align-items: center;
    background-color: $primary;
    color: $secondary;
    display: flex;
    flex-flow: row nowrap;
    height: 4rem;
    justify-content: space-around;
    list-style: none;
    width: 100vw;

    &__fixed{
      position: fixed;
      z-index: 1;

      &-top{
        left: 0;
        top:0;
      }
    }
    &__item{
      color: blue;
      padding: 0;

      & a, a:link, a:visited, a:hover, a:active{
          text-decoration: none;
      }
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
