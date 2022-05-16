<template>
  <div class="_container">
    <div class="container-fluid">
      <div class="row">
        <div v-for="(Comic, index) in dcComics" :key="index" class="col-2">
        
          <img :src="Comic.thumb" :alt="Comic.series">
          <div class="title">{{Comic.series}}</div>

        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardsComponent',
}
</script>

<style>

</style>