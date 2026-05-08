<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<view class="text">
				<text class="title">{{ok? title:title2}}</text>
			</view>
			
			<view class="bottun">
				<button :type="buttontype" @click="change">你是高手吗</button>
				<button :type="buttun2" @click="shagouchange()">Try this</button>
				<navigator url="/pages/page2/page2" open-type="navigate"><button :type="buttun2">点击跳转</button></navigator>
				<navigator url="/pages/page3/page3" open-type="navigate"><button :type="buttontype">点击跳转</button></navigator>
			</view>
			
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello',
				title2: '重生之我是uni-app啥狗',
				buttontype: "primary",
				buttun2: "success",
				ok:true
			}
		},
		onLoad() {
			this.title = 'Hello'
		},
		onHide() {
			this.title = 'Bye'
		},
		onShow() {
			this.title = 'Welcome back'
		},
		methods: {
			change(){
				this.title = '重生之我是uni-app高手'
				this.ok = !this.ok
			},
			shagouchange(){
				this.title = '你是啥狗'
			}
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
		flex-direction: column;
	}

	.title {
		display: flex;
		justify-content: center;
		font-size: 36rpx;
		color: #8f8f94;
	}
	
	.bottun {
			display: flex;
			flex-direction: column;
			gap: 15px;
			width: 200px;
		}
</style>
