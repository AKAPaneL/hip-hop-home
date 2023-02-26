<template>
	<view class="content">
		<!-- banner部分-->
		<banner></banner>
		<!-- 横向滚动菜单 -->
		<scrollNav></scrollNav>
		<!-- 推荐歌单 -->
		<recommendedPlaylist></recommendedPlaylist>
		<!-- 热门说唱 -->
		<hotRap></hotRap>
		<VirtualList></VirtualList>
	</view>
</template>

<script>
import banner from './components/banner.vue';
import scrollNav from './components/scroll-nav.vue';
import recommendedPlaylist from './components/recommended-playlist.vue';
import hotRap from './components/hot-rap.vue';
	export default {
		components:{
			banner,
			scrollNav,
			recommendedPlaylist,
			hotRap
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
