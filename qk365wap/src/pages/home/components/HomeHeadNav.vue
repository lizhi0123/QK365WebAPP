<template>
    <div class="header">
        <div class="header-left">
            <div class="header-left-city">
                上海 
            </div>
             <div class="iconfont header-left-img">
                 &#xe749;
             </div>
        </div>
            <div class="homeNav-img-div">
                <!-- 标题 -->
                <img style="width: 100%; height:100%; top: 0; left: 0;" src="@/assets/images/home_qkLogo.png">
            </div>
    </div>
    
</template>

<script >
export default {
  name: 'HomeHeadNav'
}

    
</script>

<style lang="stylus"  scoped>
@import '~@/assets/styles/varibles.styl'
$headerCityWidth = 0.8rem

.header 
    position: fixed;
    width: 100%;
    height:$navHeight;
    line-height:$navHeight;
    line-height: $navHeight;
    z-index: 9999;
    border-bottom: .01rem solid #e5e5e5

    .header-left 
        position absolute
        font-size: .28rem
        margin: auto 
        top: 0;
        bottom: 0;
        left: .2rem
        width: ($headerCityWidth + 0.3rem);
        height: .58rem
        line-height: .58rem
         // text-align: center
        // vertical-align: middle
        // color $greenTitleTextColor
        // background-color red
    
        .header-left-city
            position: absolute;
            top:0; left: 0; bottom: 0;
            width: $headerCityWidth;
            text-align: center;
            color: $greenTitleTextColor
        .header-left-img
            position absolute
            top:0; left: $headerCityWidth; bottom:0;
            width: 0.3rem;
    .homeNav-img-div 
        position: absolute;
        width: 1.4rem;
        height: .5rem;
        line-height: .25rem;
        text-align: center;
        margin: auto; 
        top: 0; left: 0; bottom: 0; right: 0;

         
                  
</style>
