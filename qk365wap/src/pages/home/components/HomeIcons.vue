<template>
    <div class="homeIcon">
        <div class="topSpace">
        </div>
        <div class="iconContent">
            <div class="icon" v-for="iconItem of iconList" :key="iconItem.id">
                <div class="icon-img">
                    <img class="icon-img-content" src="http://oss-wuxi.qk365.com/qingkepic/M00/73/45/CgoKaFtpK1uAHQiPAAAMPSqyXRU977.png" />
                </div>
                <p class="icon-desc">{{iconItem.title}}</p>
            </div>
        </div>
        
    </div>

</template>

<script>
export default {
  name: 'HomeIcons',
  props: {
    list: Array
  },
  data () {
    return {
        iconList: [{
            id: '001',
            title: '标题1'
        },
        {
            id: '002',
            title: '标题2'
        },{
            id: '003',
            title: '标题3'
        },
        {
            id: '004',
            title: '标题4'
        },{
            id: '005',
            title: '标题5'
        },
        {
            id: '006',
            title: '标题6'
        },{
            id: '007',
            title: '标题7'
        },
        {
            id: '008',
            title: '标题8'
        }]
    }
  },
  computed: {

  }
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