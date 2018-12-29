<template>
    <div class="header">
        <div class="header-left">
            返回
        </div>
    </div>
    
</template>

<script >
export default {
  name: 'HomeHeadNav'
}

    
</script>

<style lang="stylus"  scoped>
.header
    position: fixed
    left:0
    top:0
    height:.84rem
    width: 100%
    z-index: 9999
    // display: flex
    background: #FC7F08FF
    // margin-top: .0rem
    // margin-left: .0rem
    // height: .86rem
    // width: 100%
    // position: relative 
    .header-left
        // float: left
        margin-top: .2rem
        // padding-left: .64rem
        margin-left: .2rem
        width: .84rem
        height: .58rem
        line-height: .58rem
        text-align: center
        vertical-align: middle
        background: #21FE06FF
</style>
