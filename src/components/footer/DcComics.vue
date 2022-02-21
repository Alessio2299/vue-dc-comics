<template>
  <div class="listNav">
    <ul>
      <li class="titleList">{{nameList}}</li>
      <li v-for="(item,index) in listNavFooter" :key="index">
        <a :href="item.url">{{item.name}}</a>
      </li>
   </ul>
  <ShopNav />
  </div>
</template>

<script>
import ShopNav from "./ShopNav.vue";
export default {
  name: 'DcComics',
  components: {
    ShopNav
  },
  data: function(){
    return{
      nameList: "DcComics",
      listNavFooter:[
        {
          name: "Character",
          url: "#"
        },
        {
          name: "Comics",
          url: "#"
        },
        {
          name: "Movies",
          url: "#"
        },
        {
          name: "Tv",
          url: "#"
        },
        {
          name: "Games",
          url: "#"
        },
        {
          name: "Videos",
          url: "#"
        },
        {
          name: "News",
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
    margin-right: 20px;
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
