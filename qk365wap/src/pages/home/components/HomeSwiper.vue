<template>
  <swiper :options="swiperOption" >
        <swiper-slide class="swiper-slide">
          <a href="http://www.baidu.com">
            <img class="swiper-img" src="http://oss-wuxi.qk365.com/qingkepic/M00/82/46/CgoKaFwtYpOAacw4AAHDBhOFINE421.png" />
          </a>
        </swiper-slide>
        <swiper-slide class="swiper-slide">
          <a href="http://www.baidu.com">
            <img class="swiper-img" src="http://oss-wuxi.qk365.com/qingkepic/M00/7D/CC/CgoKZ1wnSqyAAN8XAAH8uyVWIuY925.jpg" />
          </a>
        </swiper-slide>
        <swiper-slide class="swiper-slide">
          <a href="http://www.baidu.com">
            <img class="swiper-img" src="http://oss-wuxi.qk365.com/qingkepic/M00/82/E3/CgoKaFwt4w6ACZaZAAHu3p28mXs975.jpg" />
          </a>
        </swiper-slide>
        <swiper-slide class="swiper-slide">
          <a href="http://www.baidu.com">
            <img class="swiper-img" src="http://oss-wuxi.qk365.com/qingkepic/M00/82/55/CgoKaFwtdL-AW6xhAAP3Jr8FZAo947.jpg" />
          </a>
        </swiper-slide>
        <div class="swiper-pagination" slot="pagination"></div>
      </swiper>
</template>

<script >
import 'swiper/dist/css/swiper.css'    //在全局没引入，这里记得要！
import { swiper, swiperSlide } from 'vue-awesome-swiper'

export default {
  name: 'HomeSwiper',
  data () {
    return {
        swiperOption: {
          pagination: {
            el: '.swiper-pagination'
          }
        }
      }
  }
}
</script>

<style lang="stylus" scoped="">
  .swiper-slide
    position:relative;
    width: 100%
    height: 0
    padding-bottom: 45%
    background-color: red
    .swiper-img
      position:absolute;
      top: 0;
      left: 0;
      width: 100%
      height: 100%
      background-color: blue
    
</style>
