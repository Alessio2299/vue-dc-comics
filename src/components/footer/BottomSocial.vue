<template>
  <div class="container-social">
   <span>Follow us</span>
   <img v-for="(social,index) in listSocials" :key="index" :src="social.image" alt="">
  </div>
</template>

<script>
import logoFacebook from "../../assets/img/footer-facebook.png";
import logoTwitter from "../../assets/img/footer-twitter.png";
import logoYoutube from "../../assets/img/footer-youtube.png";
import logoPinterest from "../../assets/img/footer-pinterest.png";
import logoPeriscope from "../../assets/img/footer-periscope.png";


export default {
  name: 'BottomSocial',
  data: function(){
    return{
      listSocials:[
        {
          name: "Facebook",
          image: logoFacebook,
        },
        {
          name: "Twitter",
          image: logoTwitter,
        },
        {
          name: "Youtube",
          image: logoYoutube,
        },
        {
          name: "Pinterest",
          image: logoPinterest,
        },
        {
          name: "Periscope",
          image: logoPeriscope,
        },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  .container-social{
    text-transform: uppercase;
    font-size: 20px;
    font-weight: 600;
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 40%;
    color: rgb(5, 130, 249);
  }
</style>
