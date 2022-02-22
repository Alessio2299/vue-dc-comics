<template>
  <div class="card">
    <div class="card-img">
      <img :src="serie.thumb" :alt="serie.series">
    </div>
    <h4>{{serie.series}}</h4>
  </div>
</template>

<script>
  export default {
    name: "SingleCard",
    props: {
      serie: Object
    }
}
</script>

<style scoped lang="scss">
  .card{
    width: 150px;
    padding: 15px 2px;
    margin: 9px;
    cursor: pointer;
    .card-img{
      height: 150px;
      width: 100%;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
      }
    }
    h4{
      font-size: 11px;
      font-weight: 400;
      text-transform: uppercase;
      padding-top: 15px;
    }
  }
</style>