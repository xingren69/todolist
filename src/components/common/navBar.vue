<template>
	<div>
		<header id="header" class="mui-bar mui-bar-transparent">
			<a class="mui-action-back mui-icon mui-icon-left-nav mui-pull-left" @click='goback'></a>
			<h1 class="mui-title">{{title}}</h1>
		</header>
	</div>
</template>
<script>
	export default{
		data(){
			return{

			}
		},
		props:['title'],
		methods:{
			goback(){
				this.$router.go(-1);
			}
		}
	}
</script>
<style scoped>
	.mui-bar.mui-bar-transparent{position: relative;
		background: #e7e7e7}

</style>