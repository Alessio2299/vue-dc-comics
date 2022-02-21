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
  @import "../../assets/style/footerNav.scss";
</style>
