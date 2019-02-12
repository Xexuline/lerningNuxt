<template>
  <section class="container">
    <Header />
    <div class="offer-container">
      <Finder :offers="0"/>
    </div>
    <Footer />
  </section>
</template>

<script>

import Footer from '~/components/Footer.vue'
import Header from '~/components/Header.vue'
import Finder from '~/components/Finder.vue'

export default {
  components: {
    Header,
    Footer,
    Finder,
  },
  methods: {

  },
}
</script>

<style lang="scss">
@font-face {
  font-family: 'FontAwesome';
  src:  require('static/fonts/fa-solid-900.woff') format('woff'),
        require('static/fonts/fa-solid-900.woff2') format('woff2'),
}
.container {
  margin: 0 auto;
  min-height: 100vh;
  box-sizing: border-box;
  width: 100%;
  max-width: 154rem;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.offer-container{
  // min-height: 120vh;
  position: absolute;
  top: 6rem;
  width: 90%;
  max-height: calc(100vh - 100px);
}
.fa{
  font-family: 'FontAwesome';
  &-heart{
    &::before{
      content: "\f004";
    }
  }
  &-code{
    &::before{
      content: "\f121";
    }
  }
  &-search{
    &::before{
      content: "\f002"
    }
  }
}

</style>
