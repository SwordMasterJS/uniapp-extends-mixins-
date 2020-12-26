<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
		<view><text class="title">{{testval}}:可以继承变量</text></view>
		<view><button @click="testFunction">可以继承方法</button></view>
		<view>
			<!-- 无法继承组件 -->
			<test-comp></test-comp>
		</view>
	</view>
</template>

<script>
	// import TestComp from "@/pages/components/TestComp.vue"
	import base from "@/pages/common/base.vue"
	export default {
		mixins:[base],
		data() {
			return {
				title: 'Hello'
			}
		},
		// components: {
		//   TestComp,
		// },
		onLoad() {

		},
		methods: {

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
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
