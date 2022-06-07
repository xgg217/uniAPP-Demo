<template>
	<view class="warpp">
		<view class="box">
			<slot name="main"></slot>
		</view>
		<uni-icons type="forward" size="24" color="#999"></uni-icons>
	</view>
</template>

<script lang="ts">
</script>

<style lang="scss" scoped>
.warpp {
	display: flex;
	align-content: center;
	justify-content: space-between;
	margin-bottom: 20rpx;
	padding: 30rpx;
	background-color: #fff;
}
</style>
