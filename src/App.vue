<template>
	<h1 @click=onclick>{{ message }}</h1>
</template>

<script>
export default {
	data() {
		return {
			message: 'hello, world!',
			clickCount: 0,
		};
	},
	methods: {
		onclick() {
			this.clickCount++;
			if (this.clickCount%2 == 0) {
				this.message = 'hello, world!';
			} else {
				this.message = 'hello, cordova!';
			}
		},
	},
}
</script>
