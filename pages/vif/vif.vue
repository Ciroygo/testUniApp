<template>
	<view>
		<!-- v-if 与 v-show  钱  -->
		<view v-if="isShow">This isShow</view>
		
		<view v-else>看不见我</view>
		
		<view v-show="isShow">vshow </view>
		
		<view v-if="sex == 1 ">男</view>
		<view v-else-if="sex ==  0">女</view>
		<view v-else>
			未知
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				isShow: true,
				sex: 3,
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
