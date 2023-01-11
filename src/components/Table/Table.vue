<template>
	<div class="container-tableWithFooter">
		<table class="table" id="table">
			<TableHeader />
			<tbody id="tbody">
				<TableBody v-for="i in 11" :key="i" :index="i" />
			</tbody>
		</table>
		<div class="container-tableFromFooter">
			<Pagination />
		</div>
	</div>
</template>

<script>
import TableBody from "./TableBody.vue";
import TableHeader from "./TableHeader.vue";
import Pagination from "../Pagination.vue";

export default {
	components: {
		TableBody,
		TableHeader,
		Pagination,
	},
};
</script>

<style scoped>
.container-tableFromFooter {
	display: flex;
	justify-content: space-between;
	height: 55px;
	align-items: center;
	background: #0f0e13 !important;
}
.container-tableWithFooter {
	display: flex;
	flex-direction: column;
}
table {
	display: block;
	height: 60vh;
	overflow-y: auto;
	position: relative;
	margin-bottom: 0;
}
table::-webkit-scrollbar {
	-webkit-appearance: none;
}

table::-webkit-scrollbar:vertical {
	width: 10px;
}

table::-webkit-scrollbar-button:increment,
table::-webkit-scrollbar-button {
	display: none;
}

table::-webkit-scrollbar:horizontal {
	height: 10px;
}

table::-webkit-scrollbar-thumb {
	background-color: #495057;
	border-radius: 20px;
}

table::-webkit-scrollbar-track {
	border-radius: 10px;
	background: #49505742;
}
tfoot {
	position: sticky;
	bottom: 0;
}
#table {
	color: #ffffff8f !important;
}
.table > tbody {
	text-align: start !important;
	color: #ffffff8f !important;
	font-size: 12px;
	border: none;
	border-bottom-width: 0.1px;
	border-bottom-color: #ffffff59;
	background: #0f0e13 !important;
}
.table > :not(caption) > * > * {
	border-bottom-width: 0.1px !important;
	border-bottom-color: #ffffff59 !important;
}
@media (max-height: 650px) {
	table {
		height: 50vh;
	}
}
@media (min-width: 1280px) {
	table {
		height: 55vh;
	}
	.table > tbody {
		font-size: 14px;
	}
}
@media (min-width: 1400px) {
	table {
		height: 65vh;
	}
}

@media (min-width: 1650px) {
	table {
		height: 48vh;
	}
}
</style>
