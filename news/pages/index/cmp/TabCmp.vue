<template>
	<view class="warpp">
		<scroll-view :scroll-x="true" class="scroll">
			<view class="box">
				<template v-for="item of titleArr" :key="item.index">
					<text
						:class="(ind === item.index) ? 'red' : ''"
						@click="handlerPage(item.index)"
					>{{ item.name }}</text>
				</template>
			</view>
		</scroll-view>
		<view class="set">
			<uni-icons type="gear" size="30" color="#999"></uni-icons>
		</view>

	</view>
</template>

<script lang="ts" setup>
	import { readonly, ref } from 'vue';
	
	const arr = [
		{
			index: 0,
			name: '全部'
		},{
			index: 1,
			name: '前端开发'
		},{
			index: 2,
			name: '后端开发'
		},{
			index: 3,
			name: '移动开发'
		},{
			index: 4,
			name: '职场生活'
		},{
			index: 5,
			name: '精彩直播'
		},{
			index: 6,
			name: '每日一题'
		}
	]
	const titleArr = readonly(arr);
	const ind = ref(0);
	
	const handlerPage = (index) => {
		ind.value = index;
		console.log(index)
	}
	
</script>

<style scoped lang="scss">
	.warpp {
		display: flex;
		align-items: center;
		justify-content: space-between;
		border-bottom: 1rpx solid #f5f5f5;
	}

	.scroll {
		width: 90vw;

		.box {
			height: 100rpx;
			display: flex;
			align-items: center;

			text {
				padding: 0 15rpx;
				margin-right: 10rpx;
				font-size: 30rpx;
				
			}
			text:first-child {
				margin-left: 10rpx;
			}
			
			.red {
				color: red;
			}
		}
	}

	.set {
		display: flex;
		align-content: center;
		justify-content: space-between;
		padding: 5rpx 0;
	}
</style>
