<template>
	<div class="form-floating mb-3">
		<input type="text" class="form-control" :v-model="InputModel" :id="InputTxtId" placeholder="floatingInput" />
		<label for="floatingInput"
			><b>{{ InputTxtCaption }}</b></label
		>
	</div>
</template>
<script>
export default {
	name: "InputText",
	data() {
		return {}
	},
	props: {
		InputModel: String,
		InputTxtId: String,
		InputTxtCaption: String,
		InputTxtModel: String,
	},
}
</script>
