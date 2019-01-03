<template>
 <div class="container-warp" ref="containerWarp">
    <home-head-nav> </home-head-nav>
    <div class="container-scroll">
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
    </div>
 </div>
</template>

<script>
    import HomeHeadNav from './components/HomeHeadNav.vue'
export default {
  name: 'Home',
  components: {
    HomeHeadNav
  },
  data (){
    return {
        clientWidth:'',
        clientHeight:''
    }
  },
  mounted (){
    // this.clientHeight = '${document.documentElement.clientHeight}'
    this.clientHeight = document.documentElement.clientHeight;
    this.clientWidth = document.documentElement.clientWidth;
     this.$refs.containerWarp.style.height = this.clientHeight+'px';
      this.$refs.containerWarp.style.width = this.clientWidth+'px';

    // window.onresize = function temp() {
    //     this.clientHeight = document.documentElement.clientHeight;
    //     this.clientWidth =  document.documentElement.clientWidth;
    //   };
  },
   watch: {
      // // 如果 `clientHeight` 发生改变，这个函数就会运行
      // clientHeight: function () {
      //   this.changeClientHeightFixed(this.clientHeight);
      // },
      // clientWidth: function () {
      //   this.changeClientWidthFixed(this.clientWidth);
      // }
    },
    methods:{
      changeClientHeightFixed(clientHeight){ 
      //动态修改样式
        this.$refs.containerWarp.style.height = clientHeight+'px';
        // this.$refs.containerWarp.style.height = clientHeight+'px';

      },
      changeClientWidthFixed(clientWidth){ 
        this.$refs.containerWarp.style.width = clientWidth+'px';
        // this.$refs.containerWarp.style.height = clientHeight+'px';
      },
  }
}
</script>

<style lang="stylus" scoped>
@import '~@/assets/styles/varibles.styl'
.container-warp
    width: 100%
    height: 100%
    overflow: hidden
    position: relative
    background-color: $bgColor
    color: $darkTextColor
    .container-scroll
        position: absolute
        top: $navHeight
        bottom: 0rem
        left: 0rem
        right: 0rem
        overflow-y: scroll
</style>
