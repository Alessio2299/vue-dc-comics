<template>
  <div class="container">
    <div class="bottomFooter">
      <span>Sign-up Now!</span>
      <BottomSocial />
    </div>
  </div>
</template>

<script>
import BottomSocial from "./BottomSocial.vue";

export default {
  name: 'BottomFooter',
  components: {
    BottomSocial
  }
}
</script>

<style scoped lang="scss">
  .container{
    background-color: rgb(48, 48, 48);
    .bottomFooter{
      width: 70%;
      margin: auto;
      padding: 40px 0;
      display: flex;
      justify-content: space-between;
      align-items: center;
      span{
        text-transform: uppercase;
        border: 2px solid rgb(5, 130, 249);
        padding: 10px;
        font-size: 20px;
        color: #fff;
      }
    }
  }
</style>
