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
		console.log('show_page2');
	})
	onShow(function(){
		console.log("page2页面显示");
	})
	onunload(()=>{
		console.log("unload_page2")
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
