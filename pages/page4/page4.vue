<template>
	<view class="content">
		<view class="bg-img"></view>
	</view>
	
</template>

<script setup>
	
</script>

<style>
	.content{
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.bg-img{
		width: 200rpx;
		height: 200rpx;
		background-image: url(~@/static/logo.png);
		/*~@转换图片为base64,
		如果微信小程序中图片>40kb无法自动转换成base64，
		则会有显示异常的状况，需要用转换器手动转换图片格式*/
		background-size: 100%;
	}
</style>
