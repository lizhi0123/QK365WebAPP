<template>
  <!-- <div class="wrapper"> -->
    <swiper :options="swiperOption" class="wrapper">
      <swiper-slide >
        <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1812/e0/7aed5dde53dabe02.jpg_750x200_9b7a65fd.jpg" />
    </swiper-slide>
    <swiper-slide >
        <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1811/7c/8e5c4ab8ee8b7402.jpg_750x200_dd7a38dd.jpg" />
    </swiper-slide>
          <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  <!-- </div> -->
</template>

<script >
export default {
  name: 'HomeSwiper'
}
</script>

<style lang="stylus" scoped="">
.wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 31.25%
    background: #eee
   .swiper-img
    width: 100%
</style>
