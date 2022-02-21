<template>
  <div class="navFooter">
    <div class="container">
      <DcComics />
      <DcNav />
      <SitesNav />
      <ShopNav />
    </div>
  </div>
</template>

<script>
import DcComics from "./DcComics.vue";
import DcNav from "./DcNav.vue";
import SitesNav from "./SitesNav.vue";
import ShopNav from "./ShopNav.vue";

export default {
  name: 'NavFooter',
   components: {
    DcComics,
    DcNav,
    SitesNav,
    ShopNav
  }
}
</script>

<style scoped lang="scss">
  .navFooter{
    background-image: url("../../assets/img/footer-bg.jpg");
    .container{
      width: 70%;
      margin: auto;
      display: flex;
    }
  }
</style>
