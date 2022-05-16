<template>
  <header>
    <div class="_container d-flex justify-content-between align-items-center">
      
        
          <div class="d-flex align-items-center"><img src="../assets/img/dc-logo.png" alt=""></div>
          <ul>
            <li v-for="(link, index) in headMenu"
              :key="`headMenu-${index}`">
              <a :class="{ 'active' : linkAttivo == index}" :href="link.source">{{ link.text }}</a>
            </li>
          </ul>
        
      
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent',

  data() {
    return {

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
      
    img {
      max-width: 80px;
    }

    ul {
      text-align: right;

      li {
        display: inline-block;

        a {
          margin: 0 10px;
          text-transform: uppercase;
          font-size: .7rem;

          &:focus {
            padding-bottom: 49px;
            border-bottom: 5px solid $dc-color;
            color: $dc-color;
          }
        }
      }
    }
  }
</style>