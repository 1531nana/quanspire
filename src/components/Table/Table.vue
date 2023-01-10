<template>
	<div class="container-tableWithFooter">
		<table class="table table-fixed" id="table">
			<thead class="t-head">
				<!-- <thead class="table-dark"> -->
				<tr>
					<th scope="col">
						<div class="containerTheadTh" style="gap: 5px">
							Actions
							<img src="../../assets/arrows.svg" alt="" />
						</div>
					</th>
					<th scope="col">
						<div class="containerTheadTh">
							Code <img src="../../assets/arrows.svg" alt="" />
							<img src="../../assets/filter.svg" alt="" />
						</div>
					</th>
					<th scope="col">
						<div class="containerTheadTh">
							Portfolio <img src="../../assets/arrows.svg" alt="" />
							<img src="../../assets/filter.svg" alt="" />
						</div>
					</th>

					<th scope="col" class="text-center">
						<div class="containerTheadTh">
							Rate <img src="../../assets/arrows.svg" alt="" />
							<img src="../../assets/filter.svg" alt="" />
						</div>
					</th>
					<th scope="col">
						<div class="containerTheadTh">
							Exposure Type <img src="../../assets/arrows.svg" alt="" />
							<img src="../../assets/filter.svg" alt="" />
						</div>
					</th>
					<th scope="col">
						<div class="containerTheadTh">
							Notional <img src="../../assets/arrows.svg" alt="" />
							<img src="../../assets/filter.svg" alt="" />
						</div>
					</th>
					<th scope="col">
						<div class="containerTheadTh">
							Currency <img src="../../assets/arrows.svg" alt="" />
							<img src="../../assets/filter.svg" alt="" />
						</div>
					</th>
					<th scope="col">
						<div class="containerTheadTh">
							Expected Cash Flow Date
							<img src="../../assets/arrows.svg" alt="" />
							<img src="../../assets/filter.svg" alt="" />
						</div>
					</th>
					<th scope="col">
						<div class="containerTheadTh">
							Issue Date <img src="../../assets/arrows.svg" alt="" />
							<img src="../../assets/filter.svg" alt="" />
						</div>
					</th>
					<th scope="col">
						<div class="containerTheadTh">
							Rate at Issue Date <img src="../../assets/arrows.svg" alt="" />
							<img src="../../assets/filter.svg" alt="" />
						</div>
					</th>
					<th scope="col">
						<div class="containerTheadTh">
							Invoce Due Date <img src="../../assets/arrows.svg" alt="" />
							<img src="../../assets/filter.svg" alt="" />
						</div>
					</th>
				</tr>
			</thead>
			<tbody id="tbody">
				<TableBody v-for="i in 11" :key="i" :index="i" />
			</tbody>
		</table>
		<div class="container-tableFromFooter">
			<TableFooter />
		</div>
	</div>
</template>

<script>
import TableBody from "./TableBody.vue";
import TableFooter from "../Pagination.vue";

export default {
	components: {
		TableBody,
		TableFooter,
	},
};
</script>

<style scoped>
.t-head {
	background: #232227;
}
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
thead {
	position: sticky;
	top: 0;
}
tfoot {
	position: sticky;
	bottom: 0;
}
img {
	width: 15px;
}
#table {
	color: #ffffff8f !important;
}
thead th {
	width: 170px;
	font-size: 12px;
	border: 1px solid #373b3e !important;
	vertical-align: middle;
	font-weight: lighter;
	color: #ffffff8f;
}
.containerTheadTh {
	display: flex;
	flex-direction: row;
	text-align: initial;
	justify-content: flex-start;
	align-items: center;
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
@media (min-width: 1280px) {
	table {
		height: 55vh;
	}
	thead th {
		font-size: 14px;
	}
	.containerTheadTh {
		padding: 5px 0;
		gap: 5px;
	}
	.table > tbody {
		font-size: 14px;
	}
}
@media (min-width: 1400px) {
	table {
		height: 65vh;
	}
	thead th {
		font-size: 16px;
	}
	img {
		width: 16px;
	}
}

@media (min-width: 1650px) {
	table {
		height: 48vh;
	}
}

/* paleta de colores

black: negro
#0F0E13 : negro un poco más claro
#232227: gris oscuro
#ffffff8f : letra, gris más claro
#2c4190 : azul 

*/
</style>
