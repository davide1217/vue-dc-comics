<template>
  <main>
    <div class="_container">
      <div class="container-fluid">
        <div class="row">
          <div class="col-12"><h2> -- content goes here --</h2></div>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'MainComponent'
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