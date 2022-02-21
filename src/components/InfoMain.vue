<template>
  <section class="info">
    <div class="content-info">
      <div v-for="(info,index) in listInfo" :key="index" class="card">
        <img :src="'../assets/img/' + info.image " :alt="info.name">
        <span>{{info.name}}</span>
        
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'InfoMain',
  data: function (){
    return{
      listInfo:[
        {
          name: "Digital Comics",
          image: "dc-logo.png"
        },
        {
          name: "DC Merchandise",
          image: "buy-comics-merchandise.png"
        },
        {
          name: "Subscription",
          image: "buy-comics-subscriptions.png"
        },
        {
          name: "Comic Shop Locator",
          image: "buy-comics-shop-locator.png"
        },
        {
          name: "DC Power Visa",
          image: "buy-dc-power-visa.png"
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
.info{
  background-color: rgb(5, 130, 249);
  height: 200px;
  .content-info{
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 70%;
    margin: auto;
    .card{
      height: 70px;
      img{
        height: 100%;
        vertical-align: middle;
      }
      span{
        color: #fff;
        text-transform: uppercase;
        margin-left: 10px;
        font-size: 13px;
      }
    }
  }
}
</style>
