<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
			<input type="text" :value="title" @input="change">
		</view>
		<navigator url="../hello/hello">
			<view>
				I am {{student.age+1}} year old <br>
				I have skills such as: {{skill[0]}},{{skill[1]}},{{skill[2]}},{{skill[3]}}
			</view>
		</navigator>

	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'ciroygo test',
				student: {
					age: 18
				},
				skill: ['Java', 'HTML', 'css', 'springcloud', 'vue']
			}
		},
		onLoad() {

		},
		methods: {
			change(e) {
				var txtTitle = e.detail.value;
				this.title = txtTitle;
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
		height: 200upx;
		width: 200upx;
		margin-top: 200upx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50upx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36upx;
		color: #8f8f94;
	}
</style>
