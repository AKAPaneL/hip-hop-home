<template>
  <view class="recommendedPlaylist-container">
    <view class="card-box">
        <view class="title">推荐歌单</view>
        <view class="content">
            <view class="datail" v-for="item in playList" :key="item" @click="handleClick">
                <view class="single-img"></view>
                <text class="dp-block">{{ item.title }}</text>
            </view>
        </view>
    </view>
  </view>
</template>
<script>
export default {
    data(){
        return{
            playList:[
                {id:1,title:'热狗MC Hotdog'},
                {id:2,title:'中国说唱巅峰对决'},
                {id:3,title:'Beat 多为 Boom Bap free 欢迎投稿'}
            ]
        }
    },
    methods:{
        handleClick(){
            // 处理点击
            console.log('点击歌单');
        }
    }
}
</script>
<style scoped lang="scss">
.recommendedPlaylist-container{
    width: 100vw;
    padding: 4vw 0;
}
.dp-block{
    display: block;
}
.card-box{
    .title{
        font-size: 4.267vw;
        font-weight: 700;
        padding-left: 4vw;
        margin-bottom: 3vw;
    }
    .content{
        display: flex;
        justify-content: space-between;
        font-size: 2.667vw;
        padding: 0 4vw;
    }
    .datail{
        width: 29vw;
    }
    .datail .single-img{
        width: 29vw;
        height: 29vw;
        background-color: #f1f2f6;
        border-radius: 2.5vw;
        overflow:hidden;
    }
    .datail text{
        margin-top:2.667vw;
    }
}
</style>