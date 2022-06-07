<template>
	<view  class="nav-bar">
		<!-- <text>1</text> -->
		<slot name="left"></slot>
		
		<view class="self">
			<view class="ic">
				<uni-icons type="search" size="20" color="#999"></uni-icons>
				<view class="tips">
					<slot name="main"></slot>
				</view>
				
			</view>
		</view>
		
		<!-- <uni-icons type="search" color="#999"></uni-icons> -->
		<!-- <view>输入文章标题进行搜索12</view> -->
	</view>
</template>

<script setup lang="ts">
</script>

<style scoped lang="scss">
.nav-bar {
	width: 100vw;
	height: 100rpx;
	padding: 1.1vh 4vw;
	// border: 1px solid red;
	background-color: #f25037;
	display: flex;
	align-content: center;
	justify-content: space-between;
	box-sizing: border-box;
}

.self {
	width: 100%;
	border-radius: 30rpx;
	background-color: #fff;
	padding: 10rpx 3%;
	display: flex;
	align-content: center;
	
	.ic {
		display: flex;
		align-content: center;
		justify-content: center;
		// border: 1px solid red;
		margin-right: 20rpx;
	}
	
	.tips {
		margin-left: 15rpx;
	}
}
</style>
