<template>
	<div class="bo">
		<kmm></kmm>
	</div>
</template>
<script>
	import kmm from './first/kmm.vue'
	export default {
		components: {
			kmm
		}
	}
</script>
<style>
	body {
		font-family: Helvetica, sans-serif;
	}
	
	.bo {
		width: 100px;
		height: 100px;
		background: black;
		border-radius: 50%;
	}
</style>