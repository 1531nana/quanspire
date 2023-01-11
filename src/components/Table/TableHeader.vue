<template>
	<thead class="t-head">
		<tr>
			<th scope="col" v-for="(item, i) in description" :key="i">
				<div class="containerTheadTh">
					{{ item }}
					<img src="../../assets/arrows.svg" :alt="item" />
					<img src="../../assets/filter.svg" :alt="item" />
				</div>
			</th>
		</tr>
	</thead>
</template>

<script>
export default {
	data() {
		return {
			description: [
				"Actions",
				"Code",
				"Portfolio",
				"Rate",
				"Exposure Type",
				"Notional",
				"Currency",
				"Expected Cash Flow Date",
				"Issue Date",
				"Rate at Issue Date",
				"Invoce Due Date",
			],
		};
	},
};
</script>

<style scoped>
th:first-child img:last-child {
	display: none;
}
.t-head {
	background: #232227;
}
thead {
	position: sticky;
	top: 0;
}
img {
	width: 15px;
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
