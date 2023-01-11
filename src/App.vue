<template>
	<Header />
	<Dropdown />
	<Actions />
	<Table />
	<Tabs />
</template>

<script>
import Header from "./components/Header.vue";
import Dropdown from "./components/Dropdown.vue";
import Tabs from "./components/Tabs.vue";
import Actions from "./components/Actions.vue";
import Table from "./components/Table/Table.vue";

export default {
	name: "App",
	components: {
		Header,
		Dropdown,
		Actions,
		Table,
		Tabs,
	},
};
</script>

<style>
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #ffffff8f;
}
</style>
