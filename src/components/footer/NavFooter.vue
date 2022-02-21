<template>
  <div class="navList">
    <div class="navFooter">
      <div class="container">
        <DcComics />
        <DcNav />
        <SitesNav />
      </div>
      <img src="../../assets/img/dc-logo-bg.png">
    </div>
  </div>
</template>

<script>
import DcComics from "./DcComics.vue";
import DcNav from "./DcNav.vue";
import SitesNav from "./SitesNav.vue";

export default {
  name: 'NavFooter',
   components: {
    DcComics,
    DcNav,
    SitesNav,
  }
}
</script>

<style scoped lang="scss">
  .navList{
    background-image: url("../../assets/img/footer-bg.jpg");
    height: 420px;
    overflow: hidden;
    .navFooter{
      display: flex;
      width: 70%;
      margin: auto;
      position: relative;
      justify-content: space-between;
      .container{ 
        display: flex;
      }
      img{
        position: absolute;
        right: 0;
        transform: translateY(-10%);
      }
    }
  }
</style>
