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
  name: 'SitesNav',
  data: function(){
    return{
      nameList: "Sites",
      listNavFooter:[
        {
          name: "DC",
          url: "#"
        },
        {
          name: "MAD Magazine",
          url: "#"
        },
        {
          name: "DC Kids",
          url: "#"
        },
        {
          name: "DC Universe",
          url: "#"
        },
        {
          name: "Dc Power Visa",
          url: "#"
        },
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
