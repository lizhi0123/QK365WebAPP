<template>
    <div class="homeIcon">
        <div class="topSpace">
        </div>
        <div class="iconContent">
            <div class="icon">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">我要租房</p>
            </div>
            <div class="icon">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">账单查询</p>
            </div>
            <div class="icon">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">我要开门</p>
            </div>
            <div class="icon">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">扫一扫</p>
            </div>
            <div class="icon">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">青客优选</p>
            </div>
            <div class="icon">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">我要托管</p>
            </div>
            <div class="icon">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">电费查询</p>
            </div>
            <div class="icon">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">在线报修</p>
            </div>
            <div class="icon">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">优惠券</p>
            </div>
            <div class="icon">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">老带新</p>
            </div>

        </div>
        
    </div>

</template>

<script>
export default {
  name: 'HomeSwiper'
}
</script>

<style lang="stylus" scoped="">
.homeIcon
    position relative
    margin-top 0.2rem
    margin-bottom 0.1rem
    width: 100%
    height 0
    padding-bottom 31%
    .iconContent
        position:absolute;
        top: 0;
        left: 0;
        width: 100%
        height: 100% 
        .icon
            position relative
            float left
            width 20%
            height 50%
            .icon-img
                position absolute
                top:0
                left: 0;
                right:0
                bottom: .44rem
                padding: .1rem
                .icon-img-content
                     display: block
                     margin: 0 auto
                     height: 100%
            .icon-desc
                position: absolute
                left: 0
                right: 0
                bottom: 0
                height: .44rem
                line-height: .44rem
                text-align: center
                font-size 8px
                padding-bottom .09rem
                 
                
   
</style>