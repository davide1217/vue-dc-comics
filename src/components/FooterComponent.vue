<template>
  <footer>
    <div></div>
    <div></div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComponent'
}
</script>

<style lang="scss" scoped>
  @import "../assets/vars";

  footer {
    height: calc(100vh - 390px);
    background-color: $dc-color;
    border: 1px solid white;
    div {
      height: calc(100% - 100px);
      background-color: $dc-color;
      border: 1px solid white;
    }
    div:last-of-type {
      height: 100px;
      background-color: $dc-color;
      border: 1px solid white;
    }
  }
</style>