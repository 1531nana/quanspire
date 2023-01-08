<template>
	<table class="table table-dark table-hover">
		<thead>
			<tr>
				<th scope="col">
					<div class="containerTheadTh">
						Actions <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>
				<th scope="col">
					<div class="containerTheadTh">
						Code <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>
				<th scope="col">
					<div class="containerTheadTh">
						Portfolio <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>

				<th scope="col" class="text-center">
					<div class="containerTheadTh">
						Rate <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>
				<th scope="col">
					<div class="containerTheadTh">
						Exposure Type <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>
				<th scope="col">
					<div class="containerTheadTh">
						Notional <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>
				<th scope="col">
					<div class="containerTheadTh">
						Currency <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>
				<th scope="col">
					<div class="containerTheadTh">
						Expected Cash Flow Date <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>
				<th scope="col">
					<div class="containerTheadTh">
						Issue Date <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>
				<th scope="col">
					<div class="containerTheadTh">
						Rate at Issue Date <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>
				<th scope="col">
					<div class="containerTheadTh">
						Invoce Due Date <img src="../assets/arrows.svg" alt="" />
						<img src="../assets/filter.svg" alt="" />
					</div>
				</th>
			</tr>
		</thead>
	</table>
</template>

<style scoped>
img {
	width: 15px;
}
thead th {
	font-size: 12px;
	border: 1px solid #373b3e !important;
	vertical-align: middle;
	font-weight: lighter;
	color: #ffffffc8;
}
.containerTheadTh {
	display: flex;
	flex-direction: row;
	text-align: initial;
	justify-content: flex-start;
	align-items: center;
}
@media (min-width: 1280px) {
	thead th {
		font-size: 14px;
	}
	.containerTheadTh {
		padding: 5px 0;
		gap: 5px;
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
