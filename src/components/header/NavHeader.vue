<template>
  <nav>
    <ul>
      <li :class="(item.active == true) ? 'active' : ''" v-for="(item,index) in listNav" :key="index">
        <a :href="item.url">{{item.list}}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'NavHeader',
  data: function(){
    return {
      listNav: [
        {
          list: "Characters",
          url: "#",
          active: false
        },
        {
          list: "Comics",
          url: "#",
          active: true
        },
        {
          list: "Movies",
          url: "#",
          active: false
        },
        {
          list: "Tv",
          url: "#",
          active: false
        },
        {
          list: "Games",
          url: "#",
          active: false
        },
        {
          list: "Collectibles",
          url: "#",
          active: false
        },
        {
          list: "Videos",
          url: "#",
          active: false
        },
        {
          list: "Fans",
          url: "#",
          active: false
        },
        {
          list: "News",
          url: "#",
          active: false
        },{
          list: "Shop",
          url: "#",
          active: false
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">  
li{
  display: inline-block;
  padding: 50px 12px;
  text-transform: uppercase;
  font-size: 12px;
  font-weight: 600;
  list-style: none;
  &.active{
  position: relative;
  &:before{
    content: "";
    width: 60%;
    height: 5px;
    background-color: rgb(12,	124, 236);
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
    position: absolute;
  }
  a{
    color: rgb(12,	124, 236);
  }
} 
  a{
    text-decoration: none;
    color: #000;
  }
}
</style>
