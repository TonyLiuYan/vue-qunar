<template>
  <div>
    <home-header/>
    <home-swiper/>
    <home-icons/>
    <home-recommend/>
    <home-weekend/>
  </div>
</template>

<script>
  import HomeHeader from './components/Header'
  import HomeSwiper from './components/Swiper'
  import HomeIcons from './components/Icons'
  import HomeRecommend from './components/Recommend'
  import HomeWeekend from './components/Weekend'
  import axios from 'axios'

  export default {
    name: 'Home',
    components: {
      HomeHeader,
      HomeSwiper,
      HomeIcons,
      HomeRecommend,
      HomeWeekend
    },
    methods: {
      getHomeInfo() {
        axios.get('/api/index.json').then(this.getHomeInfoSucc)
      },
      getHomeInfoSucc(res) {
        console.log(res)
      }
    },
    mounted() {
      this.getHomeInfo()
    }
  }
</script>

<style>

</style>
