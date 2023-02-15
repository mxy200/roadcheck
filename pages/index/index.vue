<template>
	<view class="indexContainer">
		<view class="header">
			<image class="logo" src="../../static/logo.png" mode=""></image>
			<view class="search">
				<image class="sousuo" src="../../static/search.png"></image>
				<input type="text" value="" placeholder='搜索....' placeholder-class="placeholder"/>
			</view>
			<button type="default">张</button>
		</view>
		<scroll-view class="navcroll" scroll-x="true">
			<view class="navItem active">推荐</view>
			<view class="navItem">推荐</view>
			<view class="navItem">推荐</view>
			<view class="navItem">推荐</view>
		</scroll-view>

	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang='stylus'>
	.indexContainer
		.header
			display flex
			padding 0rpx 5rpx
			.logo
				width 140rpx
				height 60rpx
			.search
				width 420rpx
				height 60rpx
				background #f5f5f5
				position relative
				.sousuo
					width 50rpx
					height 50rpx
					padding-top 5rpx
					position absolute
				input
					width 360rpx
					height 60prx
					border 1rpx solid #ccc
					border-color #f5f5f5
					margin-left 60rpx
					.placeholder
						font-size 40rpx
						color #333
			button
				width 144rpx
				height 60rpx
				line-height 60rpx
				text-align center
				font-size 26rpx
				padding 0 4rpx
				
		.navcroll
			display: flex
			white-space: nowrap/* 不换行 */
			.navItem
				display: inline-block
				height 40rpx
				padding: 10rpx
				font-size: 24rpx
				&.active
					border-bottom: 3rpx solid #BB2C08

</style>
