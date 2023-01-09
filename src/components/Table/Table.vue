<template>
	<table class="table table-fixed " id="table">
		<thead class="table-dark">
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
						Expected Cash Flow Date <img src="../../assets/arrows.svg" alt="" />
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
		<tbody id="tbody" style="background: #0000009e !important">
			<TableBody v-for="i in 11" :key="i" :index="i" />
		</tbody>
		<tfoot style="background: rgb(13 13 13 / 97%)">
			<TableFooter/>
		</tfoot>
	</table>
	
</template>

<script>
import TableBody from "./TableBody.vue";
import TableFooter from "./TableFooter.vue";


export default {
	components: {
		TableBody,
		TableFooter,
	},
};
</script>

<style scoped>
img {
	width: 15px;
}
#table{
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
.table>tbody {
	text-align: start !important;
	color: #ffffff8f !important;
	font-size: 12px;
	border: none;
  border-bottom-width: 0.1px;
  border-bottom-color: #ffffff59;
}
.table>:not(caption)>*>*{
	border-bottom-width: 0.1px !important;
    border-bottom-color: #ffffff59 !important;
}
@media (min-width: 1280px) {
	thead th {
		font-size: 14px;
	}
	.containerTheadTh {
		padding: 5px 0;
		gap: 5px;
	}
	.table>tbody{
		font-size: 14px;
	}
}
@media (min-width: 1400px) {
	thead th {
		font-size: 16px;
	}
	img {
		width: 16px;
	}
}
</style>
