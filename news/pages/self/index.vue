<template>
	<view class="war">
		<RowLink>
			<template v-slot:main>
				<view class="link">
					<uni-icons class="ic" type="contact" size="20" color="#999"></uni-icons>
					<text>我的文章</text>
				</view>
				
			</template>
		</RowLink>
		<RowLink>
			<template v-slot:main>
				<view class="link">
					<uni-icons class="ic" type="contact" size="20" color="#999"></uni-icons>
					<text>我的文章</text>
				</view>
				
			</template>
		</RowLink>
		<RowLink>
			<template v-slot:main>
				<view class="link">
					<uni-icons class="ic" type="help" size="20" color="#999"></uni-icons>
					<text>我的文章</text>
				</view>
				
			</template>
		</RowLink>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style scoped lang="scss">
.war {
	height: 88vh;
	background-color: #f5f5f5;
}
.link {
	display: flex;
	align-items: center;
	
	.ic {
		margin-right: 10rpx;
	}
	
	text {
		color: #333;
		font-size: 28rpx;
	}
}

</style>
