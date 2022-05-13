<template>
  <section>
    <div class="_container">
      <div class="container-fluid">
        <div class="row">

          <div class="col _col">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            <div>digitals comics</div>
          </div>

          <div class="col _col">
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <div>dc merchandise</div>
          </div>

          <div class="col _col">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <div>subscription</div>
          </div>

          <div class="col _col">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <div>comic shop locator</div>
          </div>

          <div class="col _col">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <div>dc power visa</div>
          </div>
          
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'BlueComponent'
}
</script>

<style lang="scss" scoped>
@import "../assets/vars";
@import "../assets/global";
@import "../assets/utilities";

  section {
    height: 150px;
    background-color: $dc-color;
    border: 1px solid white;

    .row > ._col {
      width: calc(100% / 5);
      display: flex;
      align-items: center;
      text-transform: uppercase;
      padding: 0 15px;
      color: white;

      img {
      width: 30%;
      margin-right: 15px;
      }

      div {
        font-size: .6rem;
      }
    }
    
  }
</style>