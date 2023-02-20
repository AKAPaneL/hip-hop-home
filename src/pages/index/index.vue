<template>
	<view class="content">
		<view class="banner">
			<uni-swiper-dot :info="info" mode="round" :bottom="100">
				<swiper class="swiper" circular autoplay :interval="interval" :duration="duration">
					<swiper-item>
						<view class="swiper-item">A</view>
					</swiper-item>
					<swiper-item>
						<view class="swiper-item">B</view>
					</swiper-item>
					<swiper-item>
						<view class="swiper-item">C</view>
					</swiper-item>
				</swiper>
			</uni-swiper-dot>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				info:[1,2,3],
				indicatorDots: true,
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
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.banner{
		width: 100vw;
		height: 45vw;
		.swiper{
			height: 100%;
		}
		swiper-item{
			box-sizing: border-box;
			padding: 5vw;
		}
		.swiper-item{
			display: block;
			height: 100%;
			background-color:red;
		}
	}
</style>
