<template>
	<view>
		<view class="text">
			<text>Hi</text>
		</view>
	</view>
</template>

<script setup>
	import {onLoad, onShow} from '@dcloudio/uni-app'
	onLoad(()=>{
		console.log('111');
	})
	onShow(function(){
		console.log("page2页面显示");
	})
</script>

<style>
   .content {
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
   }
   
   .text{
	   display: flex;
	   flex-direction: column;
	   align-items: center;
	   justify-content: center;
   }
</style>
