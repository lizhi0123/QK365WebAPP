<template>
    <div >
        <div class="top">
            <div class="topContent">
                <div class="topGreen"></div>
                <div class="topText">
                   <p class="topText-title"> 热门房源 </p>
                   <p class="topText-detail">青客，陪你开始与这座城市的故事</p>
                </div>
            </div>
            
        
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
    position relative
    // float left
    width 100%
    height: 1.5rem
    line-height 1.5rem
    background-color: red
    .topContent
        position absolute
        top: 0
        left: 0
        bottom: 0
        right: 0
        // width:100%
        // height: 1.5rem
        // line-height 1.5rem
        // background-color: yellow
        
        .topGreen
            position: absolute;
            width: 0.12rem;
            height: 0.4rem;
            margin: auto; 
            top: 0.3rem; 
            left: 0; 
            background-color green
        .topText
            position absolute
            width:100%
            height:100%
            margin-left .18rem
            .topText-title
                position absolute
                top: 0.3rem
                width: 100%
                left: 0
                height: 0.5rem
                line-height 0.5rem
            .topText-detail
                position absolute
                left:0
                top:0.8rem
                bottom 0
                right 0
                height 0.4rem
                line-height 0.4rem
                font-size 10px
                color: #999999
        

</style>