<template>
	<view class="content">
		<!-- banner部分-->
		<banner></banner>
		<!-- 横向滚动菜单 -->
		<scrollNav></scrollNav>
	</view>
</template>

<script>
import banner from './components/banner.vue';
import scrollNav from './components/scroll-nav.vue';
	export default {
		components:{
			banner,
			scrollNav
		},
		data() {
			return {

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
</style>
