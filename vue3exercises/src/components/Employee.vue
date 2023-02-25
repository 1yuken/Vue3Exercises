<script>
	export default {
	emits: ['show', 'Jujuba', '20000    '],
	data() {
		return {
			arg1: 3,
			arg2: 4
		}
	},
	methods: {
		handle() {
		this.$emit('show', 'Jujuba', '20000');
	}
}
}
</script>
<template>
	
	<button @click="handle">click</button>
</template>