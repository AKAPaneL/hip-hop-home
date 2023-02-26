<template>
  <view class="scroll-nav-container">
    <scroll-view scroll-x class="scroll-nav">
        <view class="scroll-nav-List">
            <view v-for="item in navList" :key="item.id" class="nav-item">
                <image class="nav-img" :src="item.url" lazy-load="true"/>
                <text>{{ item.text }}</text>
            </view>
        </view>
    </scroll-view>
  </view>
  
</template>

<script>
import album from '../../../static/nav/album.png'
import myMusic from '../../../static/nav/myMusic.png'
import ranking from '../../../static/nav/ranking.png'
import video from '../../../static/nav/video.png'
export default {
    data(){
        return{
            navList:[
                {id:1,text:'热门厂牌',url:myMusic},
                {id:2,text:'专辑',url:album},
                {id:3,text:'综艺',url:video},
                {id:4,text:'歌单',url:myMusic},
                {id:5,text:'排行榜',url:ranking},
                {id:6,text:'排行榜',url:ranking}
            ]
        }
    },
    mounted(){
    }
}
</script>
<style scoped lang="scss">

.scroll-nav-container{
    width: 100vw;
    color: black;
    font-size: 12px;
}
.scroll-nav .scroll-nav-List{
    display: flex;
    align-items: center;
    height: 12vw;
    width: 120vw;
}
/* #ifdef H5 */
.scroll-nav::v-deep .uni-scroll-view::-webkit-scrollbar{
    display: none;
}
/* #endif */
.scroll-nav{
    .nav-item{
        flex-shrink: 0;
        width: 20vw;
        text-align: center;
        .nav-img{
            width: 6vw;
            height: 6vw;
            margin: 0 auto;
        }
        text{
            display: block;
        }
    }
}

</style>