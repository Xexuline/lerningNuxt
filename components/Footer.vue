<template>
  <footer>

    <p>Curratelo.es is an Open Source project <span class="fa fa-code"/> with <span class="fa fa-heart"/> by Ulises Gascón, Roberto Moriyon, Jesús Sabroso & individual contributors | GNU GPL-3.0</p>
  </footer>
</template>
<script>
export default {
  
}
</script>
<style lang="scss" scoped>
  @import '@/assets/styles/config.scss';

  footer{
    position: fixed;
    left: 0;
    bottom: 0;
    height: 4rem;
    width: 100%;
    background-color: $secondary;
    color: $muted;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  

</style>


