<template>
	<view class="banner">
		<swiper class="swiper" indicator-dots circular autoplay :interval="interval" :duration="duration">
			<swiper-item v-for="item in info" :key="item">
				<view class="swiper-item">{{ item }}</view>
			</swiper-item>
		</swiper>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				info:[1,2,3,4,5],
				interval:5000,
				duration:500
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style scoped lang="scss">
	.banner{
		width: 100vw;
		height: 35vw;
        padding: 4vw 0;
		.swiper{
			height: 100%;
		}
		swiper-item{
			box-sizing: border-box;
			padding: 0 4vw;
		}
		.swiper-item{
			display: block;
			height: 100%;
			background-color:#E91E63;
            border-radius: 3vw;
		}
	}
</style>
