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
  name: 'DcComics',
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
      &.titleList{
        text-transform: uppercase;
        padding: 30px 0 10px 0;
        font-size: 20px;
      }
      a{
        text-decoration: none;
        color: rgb(149, 149, 149);
      }
    }
  }
</style>
