<template>
  <div id="app" class="app">
     <!-- <home-head-nav> </home-head-nav> -->
     
     <div class="container-warp">
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
  }
}
</script>

<style lang="stylus" scoped>
.container-warp
    width: 7rem
    // height: 100%
    height: 14rem
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
