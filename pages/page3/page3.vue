<template>
	<view class="content">
		<view class="box">
			<view class="item"></view>
			<view class="item"></view>
			<view class="item"></view>
			<view class="item"></view>
			<view class="item"></view>
			<view class="item"></view>
		</view>
	</view>
</template>

<script setup>
	
</script>

<style>
	.content{
		display: flex;
		flex-direction: column;
		justify-content: ;
		align-items: center;
		align-content: center;
	}
	.box{
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		align-content: flex-start;
		justify-content: space-between;
		align-items: baseline;
		width: 500rpx;
		height: 500rpx;
		border: 10rpx solid skyblue;
		border-radius: 20rpx;
	}
	.item{
		border: 10rpx solid greenyellow;
		width: 70rpx;
		height: 70rpx;
		border-radius: 10rpx;
	}
</style>
