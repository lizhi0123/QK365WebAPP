<template>
 <div class="container-warp" ref="containerWarp">
    <home-head-nav> </home-head-nav>
    <div class="container-scroll">
      <home-swiper></home-swiper>
      <home-icons></home-icons>
      <div class="divSpace"> </div>
      <home-hot-rooms></home-hot-rooms>
     <p>Home Test 1<br><br><br><br><br><br> </p>
     <p><br><br><br>Home Test 2<br><br><br><br><br><br> </p>
     <p><br><br><br>Home Test 3<br><br><br><br><br><br> </p>
     <p><br><br><br>Home Test 4<br><br><br><br><br><br> </p>

        <br>
        <router-link to= "/helloworld">
            Helloworld 
        </router-link>
        <br>
        <br>
        <br>
        <br>
    </div>
 </div>
</template>

<script>
    import axios from 'axios'
    import qs from 'qs'

    import HomeHeadNav from './components/HomeHeadNav.vue'
    import VueAwesomeSwiper from 'vue-awesome-swiper'
    import HomeSwiper from './components/HomeSwiper.vue'
    import HomeIcons from './components/HomeIcons.vue'
    import HomeHotRooms from './components/HomeHotRooms.vue'

export default {
  name: 'Home',
  components: {
    HomeHeadNav,
    HomeSwiper,
    HomeIcons,
    HomeHotRooms
  },
  data (){
    return {
        clientWidth:'',
        clientHeight:''
    }
  },
  mounted (){
    this.getHomeInfo()
  },
   watch: {

    },
    methods:{
       getHomeInfo () {

        // axios.get('http://v.juhe.cn/toutiao/index?type=top&key=f1db1cefce44c93b2549b592a7fe6039')
        //   .then(this.getHomeInfoSucc);

          var data = {type: 'top',
          key:"f1db1cefce44c93b2549b592a7fe6039"};
// http://v.juhe.cn/toutiao/index
          axios.get('/toutiao/index').then(this.getHomeInfoSucc);
    },
    getHomeInfoSucc (res) {
      console.log("11111111111");
      console.log(res);
      res = res.data
      if (res.ret && res.data) {
        const data = res.data

        this.city = data.city
        this.swiperList = data.swiperList
        this.iconList = data.iconList
        this.recommendList = data.recommendList
      }
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~@/assets/styles/varibles.styl'
.container-warp
    width: 100%
    height: 100%
    background-color: $bgColor
    color: $darkTextColor
    .container-scroll
        // position: absolute
        top: $navHeight
        bottom: 0rem
        left: 0rem
        right: 0rem
        .divSpace
          width 100%
          height 0.2rem
          background-color lightgray
</style>
