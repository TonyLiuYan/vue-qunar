<template>
  <div>
    <home-header/>
    <home-swiper/>
    <home-icons/>
    <home-recommend/>
  </div>
</template>

<script>
  import HomeHeader from './components/Header'
  import HomeSwiper from './components/Swiper'
  import HomeIcons from './components/Icons'
  import HomeRecommend from './components/Recommend'

  export default {
    name: 'Home',
    components: {
      HomeHeader,
      HomeSwiper,
      HomeIcons,
      HomeRecommend
    }
  }
</script>

<style>

</style>
