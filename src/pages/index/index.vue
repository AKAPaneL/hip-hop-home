<template>
	<view class="content">
		<!-- banner部分-->
		<banner></banner>
	</view>
</template>

<script>
import banner from './components/banner.vue';
	export default {
		components:{
			banner
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
