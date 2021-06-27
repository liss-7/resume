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
					<view class="cu-avatar xl round margin-left" style="background-image:url(/static/me.png)"></view>
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
					<view class="content bg-green shadow-blur">
						<text>{{zhuanye}}</text> 
					</view>
				</view>
				<view class="cu-item cur cuIcon-roundcheckfill">
					<view class="content bg-red shadow-blur">
						<text>{{school}}</text> 
					</view>
				</view>
			<view class="cu-time">2012.9</view>
		</view>
		
		<view class="cu-bar bg-white">
			<view class="action">
				<text class="cuIcon-title text-blue"></text>专业技能
			</view>
		</view>
		
		<view class="cu-card case" :class="!isCard?'no-card':''">
			<view class="cu-item shadow">
				<view class="text-abc">
					<view class="solids-bottom padding-xs flex align-center">
						<view class="flex-sub text-left">
							<view class="solid-bottom text-df padding">熟练掌握 JAVA/J2EE 软件开发技术，掌握面向对象设计思想</view>
							<view class="solid-bottom text-df padding">熟练掌握 spring、springboot、springcloud、springMVC、mybatis、jpa、mybatis-plus 等开发框架</view>
							<view class="solid-bottom text-df padding">熟练掌握 nacos、gateway、feign、swagger2、sentinel 等 springcloud 组件</view>
							<view class="solid-bottom text-df padding">掌握 redis 缓存框架，cas 认证、shiro 权限控制等框架</view>
							<view class="solid-bottom text-df padding">掌握分布式开发框架 zookeeper、dubbo、disconf 的配置与使用</view>
							<view class="solid-bottom text-df padding">熟练使用 idea，eclipse， google 进行开发调试</view>
							<view class="solid-bottom text-df padding">熟练使用 maven 构建项目，git，svn 等版本控制工具</view>
							<view class="solid-bottom text-df padding">熟练配置 nginx、tomcat 等中间件完成部署</view>
							<view class="solid-bottom text-df padding">熟练配置并使用 mysql、oracle 等主流数据库，会根据执行计划进行基本调优</view>
							<view class="solid-bottom text-df padding">简单使用 docker 容器技术完成项目的部署</view>
							<view class="solid-bottom text-df padding">熟悉 linux 环境下中间件的安装与配置、工程的部署</view>
							<view class="solid-bottom text-df padding">熟悉 shell 脚本的编写</view>
						</view>
					</view>
				</view>
			</view>
		</view>
		
		<view class="cu-bar bg-white">
			<view class="action">
				<text class="cuIcon-title text-blue"></text>工作经历
			</view>
		</view>
		
		<view class="cu-timeline">
		
				<view class="cu-time">至今</view>
				<view class="cu-item">
					<view class="content">
						<view class="cu-capsule radius">
							<view class="cu-tag bg-cyan">销售易</view>
							<view class="cu-tag line-cyan">营销云</view>
						</view>
						<view class="margin-top">
							<text class="">1.营销云企业微信营销service owner，对接企业微信生态以及公司自有cdp；\n</text>
							<text class="">2.对接PM完成story的技术设计、接口的设计以及代码开发工作；\n</text>
						</view>
					</view>
				</view>
			
				<view class="cu-time">2020-04</view>
				<view class="cu-item">
					<view class="content">
						<view class="cu-capsule radius">
							<view class="cu-tag bg-cyan">深圳天源迪科信息技术股份有限公司</view>
							<view class="cu-tag line-cyan">运营商中心</view>
						</view>
						<view class="margin-top">
							<text>1.负责对接需求，制定研发计划，工作量的评估以及版本内容的制定与交付；\n</text>
							<text>2.解决项目中遇到的问题、难点。给组员提供技术方案；\n</text>
							<text>3.负责接口的设计，文档编写。参与客户现场培训；\n</text>			
						</view>
					</view>
				</view>
			
				<view class="cu-time">2018.4</view>
				<view class="cu-item">
					<view class="content">
						<view class="cu-capsule radius">
							<view class="cu-tag bg-cyan">上海中交海德科技股份有限公司</view>
							<view class="cu-tag line-cyan">技术部</view>
						</view>
						<view class="margin-top">
							<text>1.负责业务系统的搭建与模块的设计，代码的编写，数据库设计以及项目的部署、后期的维护；\n</text>
							<text>2.参与需求调研，文档编写，参与培训并受理客户的意见；\n</text>
						</view>
					</view>
				</view>
			
				<view class="cu-time">2016.7</view>
				
		</view>
		
		<view class="cu-bar bg-white">
			<view class="action">
				<text class="cuIcon-title text-blue"></text>项目经历
			</view>
		</view>
		
		<view class="solids-bottom padding-xs flex align-center">
			<view class="flex-sub text-center">
				<view class="solid-bottom text-df padding">专注视觉的小程序组件库</view>
				<view class="padding">页面默认字号，用于摘要或阅读文本</view>
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
