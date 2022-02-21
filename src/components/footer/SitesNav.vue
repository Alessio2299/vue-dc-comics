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
  @import "../../assets/style/footerNav.scss";
</style>
