<template>
	<view>
		<cu-custom bgColor="bg-gradual-blue" :isBack="false"><block slot="content">个人信息</block></cu-custom>
		
		<view class="padding bg-white">
			
			<view class="padding bg-white">
				<view class="flex">
					<view class="flex-sub bg-white padding-sm margin-xs radius ">岗位:{{gangwei}}</view>
					<view class="flex-sub bg-white padding-sm margin-xs radius cuIcon-location">Base:{{base}}</view>
				</view>
			</view>

			<view class="flex flex-wrap">
				<view class="basis-xs bg-white margin-xs padding-sm radius">
					<view class="cu-avatar xl round margin-left" style="background-image:url(../../static/me.png)"></view>
				</view>
				
				<view class="basis-lg bg-grey margin-xs padding-sm radius">
					<text class="cuIcon-profile">姓名:{{name}}  \n</text>
					<text class="cuIcon-phone">电话:{{phone}}  \n</text>
					<text class="cuIcon-mail">邮箱:{{mail}} \n</text>
					<text class="cuIcon-profile">工作年限:{{year}}</text>
				</view>
			</view>
			
		</view>
		
		<view class="cu-bar bg-white">
			<view class="action">
				<text class="cuIcon-title text-blue"></text>教育背景
			</view>
		</view>
		
		<view class="cu-timeline">
			<view class="cu-time">2016.7</view>
			<view class="cu-item cur cuIcon-roundcheckfill">
				<view class="content bg-red shadow-blur">
					<text>{{school}}</text> 
				</view>
			</view>
			<view class="cu-item cur cuIcon-roundcheckfill">
				<view class="content bg-green shadow-blur">
					<text>{{zhuanye}}</text> 
				</view>
			</view>
		
	
			<view class="cu-time">2012.9</view>
		</view>
		
		
	</view>
	
</template>

<script>
	export default {
		data() {
			return {
				name:'李森森',
				phone:'13149221121',
				zhuanye:'计算机科学与技术（本科）',
				school:'西安工业大学',
				mail:'361726964@qq.com',
				gangwei:'JAVA工程师',
				age:'29',
				year:'5年',
				base: '西安'
				
			}
		}
	}
</script>

<style>
</style>
