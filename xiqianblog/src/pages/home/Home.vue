<template>
   <div class="container-fluid">
      <home-header></home-header>
      <div class="row">
        <div class="col-lg-6 col-lg-offset-1" style="margin-top: 10px; padding: 0 0;">
          <home-swiper></home-swiper>
        </div>
      </div>
   </div>
</template>

<script>
import HomeHeader from './components/HomeHeader'
import HomeSwiper from './components/HomeSwiper'

export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper
  }
}
</script>

<style scoped>
</style>
