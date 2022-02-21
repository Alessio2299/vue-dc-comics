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
  ul{
    color: #fff;
    li{
      list-style: none;
      line-height: 25px;
      font-size: 15px;
      &.titleList{
        text-transform: uppercase;
        padding: 30px 0 10px 0;
        font-size: 16px;
      }
      a{
        text-decoration: none;
        color: rgb(149, 149, 149);
      }
    }
  }
</style>
