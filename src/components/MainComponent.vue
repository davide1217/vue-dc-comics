<template>
  <main>
    <div class="_container">
      <div class="container-fluid">
        <div class="row align-items-start">

          <CardItem v-for="(item, index) in dcComics" :key="`item${index}`" 
            :itemCard="item"
          />
          

        </div>
      </div>
    </div>

    <div>load more</div>
  </main>
</template>

<script>

import dcComics from '../assets/data/dcComics';
import CardItem from './CardItem.vue';



export default {
 name: 'MainComponent',
 
 components: {
  CardItem
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
    background-color: #1C1C1C;
    padding-top: 50px;
    text-align: center;

    & > div:last-child {
      display: inline-block;
      color: white;
      text-transform: uppercase;
      font-size: .8rem;
      background-color: $dc-color;
      margin: auto;
      padding: 5px 35px;
      margin: 20px 0;
    }
  }

  
</style>