<template>
  <div id="app">
    <HeaderPage />
    <MainPage />
    <InfoMain />
    <FooterPage />
  </div>
</template>

<script>
import HeaderPage from "../src/components/HeaderPage.vue";
import MainPage from "../src/components/MainPage.vue";
import InfoMain from "../src/components/InfoMain.vue";
import FooterPage from "../src/components/FooterPage.vue";

export default {
  name: 'App',
  components: {
    HeaderPage,
    MainPage,
    InfoMain,
    FooterPage
  }
}
</script>

<style lang="scss">
  @import "./assets/style/general.scss";
  @import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,300;0,400;0,500;0,700;1,100&display=swap');
  #app{
    font-family: 'Roboto', sans-serif;
  }
</style>
