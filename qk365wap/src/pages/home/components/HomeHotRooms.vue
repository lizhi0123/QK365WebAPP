<template>
    <div >
        <div class="topContent">
            <div class="topGreen"></div>
            <div class="topText-title"> 热门房源 </div>
            <div class="topText-detail">青客，陪你开始与这座城市的故事</div>
        </div>
        <!-- 列表 -->
        <div class="aRoom" v-for="roomItem of iconList" :key="roomItem.id">
            <img class="roomList-img" src="http://www.qk365.com/images/noPic_Big0.jpg" />
            <div class="aRoom_title">{{roomItem.title}}
            </div>
            <div class="aRoom_bottomLine">
            </div>
        </div>

    </div>

</template>

<script>
export default {
  name: 'HomeHotRooms',
  props: {
    list: Array
  },
  data () {
    return {
        iconList: [{
            id: '001',
            title: '标题名称1111'
        },
        {
            id: '002',
            title: '标题名称222'
        },{
            id: '003',
            title: '标题名称3333'
        },
        {
            id: '004',
            title: '标题名称4444'
        },{
            id: '005',
            title: '标题名称5555'
        },
        {
            id: '006',
            title: '标题名称66666'
        }]
    }
  },
  computed: {

  }
}
</script>

<style lang="stylus" scoped="">
.topContent
    left:0;
    right: 0
    height:1.2rem
    .topGreen
        position:relative;
        left:0;
        top:0.3rem;
        width: 0.1rem
        height:0.3rem;
        line-height: 0.3rem
        background-color:green;
    .topText-title
        position: relative;
        left:0.2rem
        top: -0.1rem;
        height:0.5rem
        line-height 0.5rem
    .topText-detail
        position:relative
        left:0.2rem
        top:-0.1rem
        height:0.5rem
        line-height 0.5rem
        font-size 8pt;
        color: darkgray;
.aRoom
    position:relative;
    width:100%
    height:2.5rem;
    .roomList-img
        padding:0.2rem;
        left:0;
        top:0;
        width: 2rem
        height:2rem
    .aRoom_title
        position: relative
        left:2.5rem;
        top:-2rem;
        width: 5rem
        height:1rem
    .aRoom_bottomLine
        position:relative;
        left:0
        right:0;
        top:-1rem;
        height:0.05rem;
        background-color:lightgray;
        
    
    
      

</style>