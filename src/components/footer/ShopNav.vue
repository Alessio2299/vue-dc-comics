<template>
  <ul>
    <li class="titleList">{{nameList}}</li>
    <li v-for="(item,index) in listNavFooter" :key="index">
      <a :href="item.url">{{item.name}}</a>
    </li>
  </ul>
</template>

<script>
export default {
  name: 'ShopNav',
  data: function(){
    return{
      nameList: "Shop",
      listNavFooter:[
        {
          name: "Shop DC",
          url: "#"
        },
        {
          name: "Shop DC Collectibles",
          url: "#"
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  @import "../../assets/style/footerNav.scss";

</style>
