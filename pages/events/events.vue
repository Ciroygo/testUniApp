<template>
	<view>
		<input type="text" style="background-color: #8F8F94;height: 100rpx;" :value="title" @input="change"
		@focus="focus"
		@blur="blur"
		
		@confirm="confirm"
		@click="click"
		@tap="tap"
		@longpress="longpress"
		>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			change() {
				console.log("文本发生变化");
			},
			focus() {
				console.log("获得焦点");
			},
			blur() {
				console.log("失去焦点");
			},
			confirm() {
				console.log("点击完成");
			},
			click() {
				console.log("被单击");
			},
			tap() {
				console.log("被触摸");
			},
			longpress() {
				console.log("长时间按住");
			}
		}
	}
</script>

<style>

</style>
