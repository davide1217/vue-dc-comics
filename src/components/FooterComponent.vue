<template>
  <footer>

    <section>
      <div class="_container d-flex">
        
        <div class="h-100">
          <div>
            <h4>dc comics</h4>
            <ul>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul>
          </div>

          <div>
            <h4>shop</h4>
            <ul>
              <li>Shop DC</li>
              <li>Shop DC Collections</li>
            </ul>
          </div>

          <div>
            <h4>dc</h4>
            <ul>
              <li>Terms Of Use</li>
              <li>Privacy policy (New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>
          </div>
          
          <div>
            <h4>dc comics</h4>
            <ul>
              <li>DC </li>
              <li>MAD Magazine </li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
          
        </div>

        <div>
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>

      </div>
    </section>

    <section>
      <div class="_container">
        <div>sign-up now</div>
        <div class="d-flex align-items-center">
          <div>follow us</div>
          <img src="../assets/img/footer-facebook.png" alt="">
          <img src="../assets/img/footer-twitter.png" alt="">
          <img src="../assets/img/footer-youtube.png" alt="">
          <img src="../assets/img/footer-pinterest.png" alt="">
          <img src="../assets/img/footer-periscope.png" alt="">
        </div>
      </div>
    </section>
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

    section:first-child {
      height: calc(100% - 100px);
      background-image: url(../assets/img/footer-bg.jpg);
      background-size: cover;
      overflow: hidden;

      ._container > div:first-child {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        padding: 30px 0;

        & > div {
          width: 100px;
        }

        h4{
          color: white;
          text-transform: uppercase;
          font-weight: bold;
          font-size: .85rem;
        }

        ul {
          padding-left: 0;

          li {
            color: #959595;
            font-size: .7rem;
          }
        }              
      }

      ._container > div:last-child {
        display: flex;
        justify-content: flex-end;
        align-items: center;
        flex-grow: 1;

        img {
          width: 500px;
        }
      }

      
    }

    section:last-child {
      height: 100px;
      background-color: #303030;

      & > ._container {
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;

        div {
          height: auto;
          text-transform: uppercase;
        }

        & > div:first-child {
          color: white;
          padding: 7px 10px;
          border: 2px solid $dc-color;
          font-size: .8rem;
        }

        & > div:last-child {

          & > div {
            color: $dc-color;
            font-size: .95rem;
            font-weight: bold;
          }

          img {
            width: 25px;
            margin-left: 15px;
          }
        }
        
      }
    }
  }
</style>