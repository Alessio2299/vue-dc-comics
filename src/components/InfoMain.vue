<template>
  <section class="info">
    <div class="content-info">
      <div v-for="(info,index) in listInfo" :key="index" class="card">
        <img :src="info.image" :alt="info.name">
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
          image: "../assets/img/buy-comics-digital-comics.png"
        },
        {
          name: "DC Merchandise",
          image: "../assets/img/buy-comics-merchandise.png"
        },
        {
          name: "Subscription",
          image: "../assets/img/buy-comics-subscriptions.png"
        },
        {
          name: "Comic Shop Locator",
          image: "../assets/img/buy-comics-shop-locator.png"
        },
        {
          name: "DC Power Visa",
          image: "../assets/img/buy-dc-power-visa.png"
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
