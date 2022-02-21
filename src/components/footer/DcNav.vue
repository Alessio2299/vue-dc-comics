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
  name: 'DcNav',
  data: function(){
    return{
      nameList: "Dc",
      listNavFooter:[
        {
          name: "Term Of Use",
          url: "#"
        },
        {
          name: "Privacy policy (New)",
          url: "#"
        },
        {
          name: "Ad Choise",
          url: "#"
        },
        {
          name: "Advertising",
          url: "#"
        },
        {
          name: "Jobs",
          url: "#"
        },
        {
          name: "Subscriptions",
          url: "#"
        },
        {
          name: "Talent Workshop",
          url: "#"
        },
        {
          name: "CPSC Certificates",
          url: "#"
        },
        {
          name: "Ratings",
          url: "#"
        },
        {
          name: "Shop Help",
          url: "#"
        },
        {
          name: "Contact Us",
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
