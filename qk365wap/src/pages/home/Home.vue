<template>
  <div id="app" class="app">
     <home-head-nav> </home-head-nav>
     <div class="container">
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
         <p><br><br><br>Home Test <br><br><br><br><br><br> </p>
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
  }
}
</script>

<style lang="stylus" scoped>
.app
    width:100%
    overflow: hidden
    background-color: yellow

</style>
