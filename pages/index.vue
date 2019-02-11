<template>
  <section class="container">
    <Header />
    <Footer />
  </section>
</template>

<script>

import Footer from '~/components/Footer.vue'
import Header from '~/components/Header.vue'

export default {
  components: {
    Header,
    Footer
  }
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
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
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
}

</style>
