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
      nameList: "Dc Comics",
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
  @import "../../assets/style/footerNav.scss";
</style>
