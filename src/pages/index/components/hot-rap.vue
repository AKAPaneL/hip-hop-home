<template>
  <view class="hot-rap-container">
    <view class="card-box">
        <view class="title">热门说唱</view>
        <view class="content">
            <view v-for="item in 3" :key="item" class="content-item">
                <view class="avatar"></view>
                <view class="font">
                    <text class="up-font dp-block"></text>
                    <text class="down-font dp-block"></text>
                </view>
            </view>
        </view>
    </view>
  </view>
</template>
<script>
export default {}
</script>
<style>

</style>