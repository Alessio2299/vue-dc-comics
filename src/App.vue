<template>
  <div id="app">
    <HeaderPage />
    <MainPage />
    <InfoMain />
  </div>
</template>

<script>
import HeaderPage from "../src/components/HeaderPage.vue";
import MainPage from "../src/components/MainPage.vue";
import InfoMain from "../src/components/InfoMain.vue";

export default {
  name: 'App',
  components: {
    HeaderPage,
    MainPage,
    InfoMain,
  }
}
</script>

<style lang="scss">
  @import "./assets/style/general.scss";
</style>
