<template>
  <nav class="nav nav__fixed nav__fixed-top">
    <ul>
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
  .nav {
    color: red;
    background-color: #009688;
    color: rgba(255,255,255,.84);
    width: 100vw;
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
  }
</style>
