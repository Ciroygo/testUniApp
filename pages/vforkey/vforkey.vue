<template>
	<view>
		<view v-for="stu in studentArray" :key="stu.id">
			<checkbox :value="stu.name" />{{stu.name}}
		</view>
		
		
		<button type="primary" @click="addStu">增加学生</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				studentArray:[
					{
						id: 1,
						name: "jack",
						age: 19,
						skill: ['Java', 'HTML', 'css', 'vue']
					},
					{
						id: 2,
						name: "roy",
						age: 12,
						skill: ['Java', 'HTML']
					},
					{
						id: 3,
						name: "lay",
						age: 22,
						skill: ['css', 'springcloud', 'vue']
					}
				]
			
			}
		},
		methods: {
			addStu() {
				var studentArray = this.studentArray;
				var newId = this.studentArray.length + 1;
				var newStu = {
					'id': newId,
					'name': "new stu" + newId,
					'age': 34
				};
				
				studentArray.unshift(newStu);
			}
		}
	}
</script>

<style>

</style>
