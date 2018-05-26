<template>
  <div>
    <home-header/>
    <home-swiper/>
    test
  </div>
</template>

<script>
  import HomeHeader from './components/Header'
  import HomeSwiper from './components/Swiper'
  export default {
    name: 'Home',
    components: {
      HomeHeader,
      HomeSwiper
    }
  }
</script>

<style>

</style>
