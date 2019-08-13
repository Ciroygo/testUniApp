<template>
	<view>
		<view v-for="(item, index) in studentArray">
			<view>{{index}}姓名:{{item.name}}</view>
			<view>年龄:{{item.age}}</view>
			<view>
				擅长技能: 
				<block v-for="(sk, skIndex) in item.skill">{{sk}},</block>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				studentArray:[
					{
						name: "jack",
						age: 19,
						skill: ['Java', 'HTML', 'css', 'vue']
					},
					{
						name: "roy",
						age: 12,
						skill: ['Java', 'HTML']
					},
					{
						name: "lay",
						age: 22,
						skill: ['css', 'springcloud', 'vue']
					},
					{
						name: "lucy",
						age: 16,
						skill: ['HTML', 'css', 'springcloud', 'vue']
					},
					{
						name: "laraoe",
						age: 91,
						skill: ['Java', 'vue']
					}
				]
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
