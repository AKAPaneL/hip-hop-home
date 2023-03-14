<template>
  <view class="hot-rap-container">
    <view class="card-box">
        <view class="title">热门说唱歌曲</view>
        <view class="content">
            <view v-for="item in hotMusicList" :key="item.id" class="content-item">
                <view class="avatar"></view>
                <view class="font">
                    <text class="up-font dp-block">{{ item.title }}</text>
                    <text class="down-font dp-block">{{ item.description }}</text>
                </view>
            </view>
        </view>
    </view>
  </view>
</template>
<script>
export default {
  data(){
    return {
      hotMusicList:[
        { id:1,img:'',title:'-----标---题------',description:'---描述---'},
        { id:2,img:'',title:'-----标---题------',description:'---描述---'},
        { id:3,img:'',title:'-----标---题------',description:'---描述---'}
      ]
    }
  }
}
</script>
<style scoped lang="scss">
.hot-rap-container{
    width: 100vw;
    padding: 4vw 0;
    border-top: 0.5px solid #e2e2e2;
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
        padding-left: 4vw;
        padding-top: 2vw;
        .content-item{
            display: flex;
            margin-top: 2.5vw;
            align-items: center;
            // padding: ;
        }
        .avatar{
            width: 12vw;
            height: 12vw;
            background-color: #f1f2f6;
            margin-right: 2.5vw;
            border-radius: 1.5vw;
        }
        .font{
            flex: 1;
            height: 100%;
            .up-font,.down-font{
                // background-color: #f1f2f6;
            }
            .up-font{
                width: 50vw;
                border-radius: 0.8vw;
                font-size: 13px;
                font-weight:700;
            }
            .down-font{
                width: 30vw;
                margin-top: 1.5vw;
                font-size: 10px;
            }
        }
    }
  }
</style>