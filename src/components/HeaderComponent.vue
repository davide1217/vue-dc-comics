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
          active: false,
        },
        {
          text: 'comics',
          source: '#',
          active: false,
        },
        {
          text: 'movies',
          source: '#',
          active: false,
        },
        {
          text: 'tv',
          source: '#',
          active: false,
        },
        {
          text: 'games',
          source: '#',
          active: false,
        },
        {
          text: 'collectibles',
          source: '#',
          active: false,
        },
        {
          text: 'videos',
          source: '#',
          active: false,
        },
        {
          text: 'fans',
          source: '#',
          active: false,
        },
        {
          text: 'news',
          source: '#',
          active: false,
        },
        {
          text: 'shop',
          source: '#',
          active: false,
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
      height: 100%;
      justify-content: space-between;
      align-items: center;

      ._row img {
        max-width: 80px;
      }

      ul {
        text-align: right;
      }
      
      ul li a {
        margin: 0 10px;
        text-transform: uppercase;
        font-size: .7rem;
      }

      ul li a.active {
        padding-bottom: 49.5px;
        border-bottom: 4px solid $dc-color;
      }
    }
  }
</style>