<template>
  <div class="jumbotron">
    <div>current series</div>
  </div>
</template>

<script>
export default {
  name: 'JumboComponent'
}
</script>

<style lang="scss" scoped>
@import "../assets/vars";

  .jumbotron {
    height: 300px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    position: relative;
    div {
      height: 10%;
      background-color: $dc-color;
      text-transform: uppercase;
      font-weight: bold;
      color: white;
      display: flex;
      align-items: center;
      padding: 20px;
      position: absolute;
      bottom: 0;
      left: 20%;
      transform: translate(0, +50%);

    }
    
  }
</style>