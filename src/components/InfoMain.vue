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
import digitalComics from "../assets/img/buy-comics-digital-comics.png";
import merchandise from "../assets/img/buy-comics-merchandise.png";
import subscription from "../assets/img/buy-comics-subscriptions.png";
import shopLocator from "../assets/img/buy-comics-shop-locator.png";
import powerVisa from "../assets/img/buy-dc-power-visa.svg";

export default {
  name: 'InfoMain',
  data: function (){
    return{
      listInfo:[
        {
          name: "Digital Comics",
          image: digitalComics
        },
        {
          name: "DC Merchandise",
          image: merchandise
        },
        {
          name: "Subscription",
          image: subscription
        },
        {
          name: "Comic Shop Locator",
          image: shopLocator
        },
        {
          name: "DC Power Visa",
          image: powerVisa
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  .info{
    background-color: rgb(5, 130, 249);
    .content-info{
      display: flex;
      justify-content: space-around;
      align-items: center;
      width: 70%;
      margin: auto;
      padding: 40px 0;
      .card{
        height: 55px;
        img{
          height: 100%;
          vertical-align: middle;
        }
        span{
          color: rgb(203, 229, 254);
          text-transform: uppercase;
          margin-left: 10px;
          font-size: 13px;
        }
      }
    }
  }
</style>
