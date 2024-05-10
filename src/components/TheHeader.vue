<script setup>
defineProps({
})
</script>

<template>
	<div class="chef">
		<div class="chef-main">
			<img class="logo" src="https://media-image1.baydn.com/storage_media_image/bmpdqn/73cb83b320b2db49e20345369dcbab1f.c69dc8680bb430cca7205e078b234bda.jpg?x-oss-process=image/quality,q_80" title="logo" alt="logo">
			<div class="nav-bar">
				<!-- 锚点跳转同页面 -->
				<a class="nav-anchor" href="#words">单词</a>
				<a class="nav-anchor" href="#read">阅读</a>
				<a class="nav-anchor" href="#listen">听力口语</a>
				<a class="nav-anchor" href="#program">编程</a>
				<!-- 外链 -->
				<a class="nav-anchor" href="https://company.shanbay.com/" target="_blank">关于公司</a>
			</div>
			<div class="login-btn-wrap">
				<el-button class="login-btn shanBei-btn">登陆/注册</el-button>
			</div>
		</div>
	</div>
</template>

<style lang="scss" scoped>
	.chef {
		width: 100%;
		height: 64px;
		background-color: #fff;
		.chef-main {
			width: 940px;
			margin: 0 auto;
			display: flex;
			align-items: center;

			.nav-bar {
				display: flex;
				margin-left: 70px;
			}
		}
	}
	.logo {
		width: 90px;
		height: 56px;
	}
	.nav-anchor {
		width: 96px;
	}
	a.nav-anchor {
		text-decoration: none;
		color: #333;
	}
	.login-btn-wrap {
		margin-left: 114px;

		.login-btn {
			font-size: 12px;
		}
	}
</style>