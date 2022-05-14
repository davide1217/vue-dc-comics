<template>
  <div>
    <HeaderComponent />
    <MainComponent />
    <BlueComponent />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import BlueComponent from './components/BlueComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    BlueComponent,
    FooterComponent,
  }
}
</script>

<style lang="scss">
  @import "./assets/vars";
  @import "./assets/global";
  @import "./assets/utilities";


  @import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');

</style>
