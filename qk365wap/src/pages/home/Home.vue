<template>
  <div id="app" class="app" ref="app">
     <!-- <home-head-nav> </home-head-nav> -->
     
     <div class="container-warp" ref="containerWarp">
        <div class="header">
            <div class="header-left">
                返回
            </div>
        </div>
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
    window.onresize = function temp() {
        this.clientHeight = document.documentElement.clientHeight;
        this.clientWidth =  document.documentElement.clientWidth;
      };
  },
   watch: {
      // 如果 `clientHeight` 发生改变，这个函数就会运行
      clientHeight: function () {
        this.changeClientHeightFixed(this.clientHeight);
      },
      clientWidth: function () {
        this.changeClientWidthFixed(this.clientWidth);
      }
    },
    methods:{
      changeClientHeightFixed(clientHeight){ 
      //动态修改样式
        this.$refs.app.style.height = clientHeight+'px';
        // this.$refs.containerWarp.style.height = clientHeight+'px';

      },
      changeClientWidthFixed(clientWidth){ 
        this.$refs.app.style.width = clientWidth+'px';
        // this.$refs.containerWarp.style.height = clientHeight+'px';
      },
  }
}
</script>

<style lang="stylus" scoped>
.container-warp
    width: 100%
    height: 100%
    // height: 14rem
    overflow: hidden
    position: relative
    background-color: red
    .header
        width: 100%
        height: .86rem
        background-color: orange
    .container-scroll
        position: absolute
        top: .96rem
        bottom: .1rem
        left: .1rem
        right: .1rem
        background-color: #FB02FEFF
        overflow-y: scroll
        
        

</style>
