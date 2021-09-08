<template>
	<button :v-on:click="ButtonClickFunction" type="button" class="btn btn-outline-primary">{{ ButtonTxt }}</button>
</template>
<script>
export default {
	name: "Button",
	data() {
		return {}
	},
	props: {
		ButtonTxt: String,
		ButtonClickFunction: Function,
	},
}
</script>
