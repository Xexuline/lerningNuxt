<template>
  <article class="finder--container">
    <h2>{{ title }}</h2>
    <div class="finder--box">
      <input type="text" class="finder--input" placeholder="Buscar por...">
      <span class="fa fa-search"></span>
    </div>
  </article>
</template>
<script>
export default {
  props:{
    offers: {type: Number, default: 0},
  },
  mounted(){
    console.log(this.props)
  },
  computed: {
    title: function(){
      return (this.offers) ? `Tenemos ${ this.offers } ofertas para tí!` : 'No hay!'
    }
  }
}
</script>
<style lang="scss" scoped>
@import '@/assets/styles/config.scss';

.finder{
  &--container{
    background-color: $secondary;
    padding: .5rem;
    box-shadow: px2rem(5) px2rem(5) px2rem(5) $muted;
    padding: px2rem(10);
  }

  &--box{
    display: flex;
    align-items: center;
    justify-content: center;
  }
  &--input{
    background-color: transparent;
    border: 0;
    border-bottom: 1px solid $muted;
    height: 2rem;
    margin: .5rem;
    width: 80%;
  }
}
</style>