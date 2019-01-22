<template>
    <div >
        <div class="top">
            <div class="topGreen"></div>
        热门房源
        </div>
    </div>

</template>

<script>
export default {
  name: 'HomeHotRooms'
}
</script>

<style lang="stylus" scoped="">
.top
    position absolute
    float left
    width 100%
    height: 1rem
    line-height 1rem
    background-color yellow
    .topGreen
        position: absolute;
        width: 0.12rem;
        height: 0.4rem;
        margin: auto; 
        top: 0.3rem; 
        left: 0; 
        background-color green

</style>