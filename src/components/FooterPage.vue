<template>
  <footer>
    <NavFooter />
    <BottomFooter />
  </footer>
</template>

<script>
import NavFooter from "./footer/NavFooter.vue";
import BottomFooter from "./footer/BottomFooter.vue"

export default {
  name: 'FooterPage',
  components: {
    NavFooter,
    BottomFooter
  }
}
</script>

<style scoped lang="scss">
  
</style>
