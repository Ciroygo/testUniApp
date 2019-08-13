<template>
	<view>
		<!-- #ifdef H5 -->
		<view>
			只在H5显示
		</view>
		<!-- #endif -->
		
		<!-- #ifdef MP-WEIXIN -->
		<view>
			只在WX显示
		</view>
		<!-- #endif -->
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

<style>

</style>
