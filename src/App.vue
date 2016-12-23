<template>
	<div id="app">
		<!--<img src="./assets/logo.png">-->
		<h1>{{ msg }}</h1>
		<el-button @click.native="startHacking">点一下</el-button>
		<div class="quan"v-if="aa">
			<div class="asda"> </div>
		</div>
		<model1 v-if=''></model1>
		<mode></mode>
		<modal></modal>
		<mod></mod>
	</div>
</template>

<script>
	import model1 from './modals/model1.vue'
	import mode from './modals/mode.vue'
	import modal from './modals/modal.vue'
	import mod from './modals/mod.vue'
	export default {
		components: {
			model1,
			mode,
			modal,
			mod
		},
		data() {
			return {
				msg: '开始使用',
				aa:true
			}
		},

		methods: {
			startHacking() {
				this.aa=!this.aa
				this.$notify({
					title: '正常',
					message: '123',
					duration: 6000
				})
			}
		}
	}
</script>

<style>
	body {
		font-family: Helvetica, sans-serif;
		text-align: center;
	}
	
	div {
		margin: 20px auto;
	}
	
	.quan {
		width: 50px;
		height: 50px;
		border: 1px solid black;
		border-radius: 50%;
	}
	
	.asda {
		width: 0px;
		height: 0px;
		border: 20px solid transparent;
		border-left-color: #ff5555;
		margin: 5px 0px 5px 18px;
	}
</style>