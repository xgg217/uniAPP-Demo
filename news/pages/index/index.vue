<template>
	<view class="content">
		<NavBar>
			<template v-slot:main>
			    <text class="nav-text" @click="handleGoSearchPage">输入文章标题进行搜索</text>
			  </template>
		</NavBar>
		<!-- 内容 -->
		<view class="main">
			<TabCmp>
			</TabCmp>
		</view>
	</view>
</template>

<script lang="ts" setup>
	import TabCmp from './cmp/TabCmp.vue';
	
	const { handleGoSearchPage } = (() => {
		// 点击去搜索页面
		const handleGoSearchPage = () => {
			uni.navigateTo({
				url: '/pages/search/index'
			})
		};
		
			
		return {
			handleGoSearchPage
		}
	})();
</script>

<style scoped>
.nav-text {
	/* border: 1px solid blue; */
	color: #999;
}
</style>
