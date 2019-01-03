<template>
    <div class="header">
        <div class="header-left iconfont">
            &#xe679; 返回 
        </div>
        <div class="homeNav-img-div">
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
.header
    position: fixed
    left:0
    top:0
    height:$navHeight
    line-height:$navHeight
    width: 100%
    z-index: 9999
    background: #33CC00FF

    .header-left
        font-size: .28rem
        // float: left
        margin-top: .2rem
        // padding-left: .64rem
        margin-left: .2rem
        width: 1.4rem
        height: .58rem
        line-height: .58rem
        text-align: center
        vertical-align: middle
        background: #21FE06FF
    .homeNav-img-div
        width .7rem
        height .25rem
        // text-align center
        background-color red
        margin: 0 auto
                  
</style>
