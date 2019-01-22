<template>
 <div class="container-warp" ref="containerWarp">
    <home-head-nav> </home-head-nav>
    <div class="container-scroll">
      <home-swiper></home-swiper>
         <p><br><br><br>Home Test 1<br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test 2<br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test 3<br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test 4<br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test 5<br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test 6<br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test 7<br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test 8<br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test 9<br><br><br><br><br><br> </p>

        Home Test
        <br>
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
    import HomeHeadNav from './components/HomeHeadNav.vue'
    import VueAwesomeSwiper from 'vue-awesome-swiper'
    import HomeSwiper from './components/HomeSwiper.vue'

export default {
  name: 'Home',
  components: {
    HomeHeadNav,
    HomeSwiper
  },
  data (){
    return {
        clientWidth:'',
        clientHeight:''
    }
  },
  mounted (){

  },
   watch: {

    },
    methods:{
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
        position: absolute
        top: $navHeight
        bottom: 0rem
        left: 0rem
        right: 0rem
</style>
