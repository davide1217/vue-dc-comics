<template>
  <div class="col-2">
    <div class="image"><img :src="itemCard.thumb" :alt="itemCard.series"></div>
    <h3>{{itemCard.series}}</h3>
  </div>
</template>

<script>
export default {
  name: 'CardItem',
  props:{
    itemCard: Object
  }
}
</script>

<style lang="scss" scoped>

@import "../assets/vars";

  div.col-2 {
    padding: 10px;
    cursor: pointer;
  }

  .image {
    height: 130px;
    overflow: hidden;
    margin-bottom: 20px;
    transition: .5s;
  }

  div.col-2:hover .image{
    margin: -10px 0 30px 0;
  }

  div.col-2:hover h3 {
    color: $dc-color;
  }

  h3 {
    font-size: .7rem;
    color: white;
    text-transform: uppercase;
  }
</style>