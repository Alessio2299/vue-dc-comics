<template>
  <header>
    <LogoHeader />
    <NavHeader />
  </header>
</template>

<script>
import LogoHeader from "./header/LogoHeader.vue";
import NavHeader from './header/NavHeader.vue';

export default {
  name: 'HeaderPage',
  components: {
    LogoHeader,
    NavHeader
  }
}
</script>

<style scoped lang="scss">
header{
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 70%;
  margin: auto;
}
</style>
