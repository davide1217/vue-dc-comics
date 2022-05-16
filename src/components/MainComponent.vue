<template>
  <main>
    <CardsComponent />
  </main>
</template>

<script>
import dcComics from '../assets/data/dcComics';
import CardsComponent from './components/CardsComponent.vue';

export default {
 name: 'MainComponent',
 components: {
   CardsComponent,
 },

  data() {
    return {
      dcComics
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/vars";
@import "../assets/global";
@import "../assets/utilities";

  main {
    height: 120px;
    background-color: black;

    .row {
      align-items: center;

      div{
      color: white;
      }
    }
  }

  
</style>