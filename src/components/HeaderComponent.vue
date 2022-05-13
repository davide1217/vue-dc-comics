<template>
  <header>
    <div class="_container">
      <div class="container-fluid">
        <div class="row _row">
          <div class="col-1 _col"><img src="../assets/img/dc-logo.png" alt=""></div>
          <ul class="col-11">
            <li v-for="(link, index) in headMenu"
              @click="linkAttivo = index "
              :key="`headMenu-${index}`">
              <a :class="{ 'active' : linkAttivo == index}" :href="link.source">{{ link.text }}</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent',

  data() {
    return {

      linkAttivo: null,

      headMenu: [
        {
          text: 'character',
          source: '#',
          
        },
        {
          text: 'comics',
          source: '#',
          
        },
        {
          text: 'movies',
          source: '#',
          
        },
        {
          text: 'tv',
          source: '#',
          
        },
        {
          text: 'games',
          source: '#',
          
        },
        {
          text: 'collectibles',
          source: '#',
          
        },
        {
          text: 'videos',
          source: '#',
          
        },
        {
          text: 'fans',
          source: '#',
          
        },
        {
          text: 'news',
          source: '#',
          
        },
        {
          text: 'shop',
          source: '#',
          
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/vars";
@import "../assets/global";
@import "../assets/utilities";

  header {
    height: 120px;

    ._row {
      justify-content: space-between;
      
      ._row img {
        max-width: 80px;
      }

      ul {
        text-align: right;

        li {

          a {
            margin: 0 10px;
            text-transform: uppercase;
            font-size: .7rem;

            &.active {
              padding-bottom: 49px;
              border-bottom: 4px solid $dc-color;
            }
          }
        }
      }
    }
  }
</style>