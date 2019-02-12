<template>
  <article class="card--container">
    <h2>{{ job.title }}</h2>
    <div class="card--box">
      {{ job.body }}
    </div>
  </article>
</template>
<script>
export default {
  props:{
    job: {
      title: '', body: '', url: ''
    },
  },
}
</script>
<style lang="scss" scoped>
@import '@/assets/styles/config.scss';

.card{
  &--container{
    box-shadow: px2rem(5) px2rem(5) px2rem(5) $muted;
    background-color: $secondary;
    margin: px2rem(10) 0;
    padding: .5rem;
    padding: px2rem(10);
    &:last-child{
      margin-bottom: 6rem;
    }
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