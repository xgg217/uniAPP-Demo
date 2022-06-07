<template>
	<view class="">
		<NavBar>
			<template v-slot:left>
				<view class="ic">
					<uni-icons @click="handlerBack" class="fs" type="back" size="30" color="#fff"></uni-icons>
				</view>
				
			</template>
			<template v-slot:main>
				<input type="text" placeholder="请输入文本" />
			</template>
		</NavBar>
	</view>
</template>

<script lang="ts" setup>
	const { handlerBack } = (() => {
		// 返回上一页
		const handlerBack = () => {
			
		};
		
			
		return {
			handlerBack
		}
	})();
</script>

<style >
.fs {
	display: flex;
	align-content: center;
	justify-content: center;
	line-height: 60rpx;
	/* border: 1px solid blue; */
	/* margin: 0 15rpx 0 0; */
}


</style>
<style class="scss" scoped>
.ic {
	display: flex;
	align-content: center;
	justify-content: center;
}


</style>
