<template>
	<div>
		<!--<img alt="Cesium logo" src="./assets/cesium-logo.jpeg" />-->
		<Navbar />
		<form>
			<InputText InputModel="todo.salesorder" InputTxtId="SalesOrder" InputTxtCaption="Sales Order #" />
			<InputText InputTxtCaption="Pick Carton ID" />
			<InputText InputTxtCaption="Warehouse" />
			<Button ButtonClickFunction="searchFulfillments" ButtonTxt="Pack" />
			<Button ButtonTxt="Unpack" />

			<input type="text" v-model="todo.description" />
		</form>
	</div>
</template>

<script>
import Navbar from "./components/Navbar.vue"
import InputText from "./components/InputText.vue"
import Button from "./components/Button.vue"

export default {
	name: "App",
	data() {
		return { todos: [], todo: {} }
	},
	components: {
		Navbar,
		InputText,
		Button,
	},
	methods: {
		searchFulfillments: () => {
			console.log("Search fulfillment")
		},
	},
}
</script>

<style></style>
