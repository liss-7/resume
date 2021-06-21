<template>
	<view>
		<cu-custom bgColor="bg-gradual-blue" :isBack="false"><block slot="content">个人信息</block></cu-custom>
		<view class="padding bg-white">

			<view class="basis-sm bg-white margin-xs padding-sm radius">
				岗位:{{gangwei}}
			</view>

			
			<view class="flex flex-wrap">
				<view class="basis-xs bg-white margin-xs padding-sm radius">
					<view class="cu-avatar xl round margin-left" style="background-image:url(../../static/me.png)"></view>
				</view>
				
				<view class="basis-lg bg-grey margin-xs padding-sm radius">
					<text>
						姓名:{{name}}  \n
						电话:{{phone}}  \n
						邮箱:{{mail}}
					</text>
				</view>
			</view>
			
		</view>
		
		
		<view class="cu-bar bg-white">
			<view class="action">
				<text class="cuIcon-title text-blue"></text>教育信息
			</view>
		</view>
		
		
	</view>
	
</template>

<script>
	export default {
		data() {
			return {
				name:'李森森',
				phone:'13149221121',
				zhuanye:'计算机科学与技术',
				school:'西安工业大学',
				mail:'361726964@qq.com',
				gangwei:'JAVA开发工程师',
				age:'29'
			}
		}
	}
</script>

<style>
</style>
