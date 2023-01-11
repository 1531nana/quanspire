<template>
	<div class="dropdown bg-black">
		<span
			>CREATE/UPDATE: <img src="../assets/update.svg" alt="" class="update"
		/></span>
		<div
			v-for="(label, index) in labels"
			:key="index"
			class="d-flex container-select"
		>
			<label for=""> {{ label }} </label>
			<button
				class="btn btn-secondary dpd-button"
				type="button"
				data-bs-toggle="dropdown"
				aria-expanded="false"
			>
				{{ buttons[index] }} <img src="../assets/select.svg" alt="" />
			</button>
			<ul class="dropdown-menu">
				<li v-for="option in options[index]" :key="option">
					<a class="dropdown-item" href="#"> {{ option }} </a>
				</li>
			</ul>
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			labels: ["COMPANY:", "PORTFOLIOS:", "CURRENCIES:"],
			buttons: ["QUANSPIRE", "1YLAYERS", "USDCOP"],
			options: [
				["SURA", "Challenger", "Acepalma"],
				["2YLAYERS"],
				["EUR", "YEN", "PEN", "MXN", "Corn", "Soya"],
			],
		};
	},
};
</script>

<style scoped>
.update {
	padding-bottom: 8px;
}
.bg-black {
	font-size: 12px;
	display: flex;
	gap: 25px;
	align-items: center;
	padding-left: 5px;
	padding: 8px;
	color: #ffffff8f !important;
}
.dpd-button {
	width: 100%;
	display: flex;
	justify-content: space-between;
	align-items: center;
	background: #0f0e13 !important;
	border-radius: 0 !important;
	padding: 5px 10px !important;
	border-width: 0 0 2px 0;
	gap: 50px;
}
button {
	font-size: 12px;
}
.dropdown-menu.show {
	font-size: 12px !important ;
}
.container-select {
	gap: 25px;
	align-items: center;
}

@media (min-width: 1280px) {
	.dpd-button {
		gap: 80px;
	}
	button {
		font-size: 14px;
	}
	.dropdown-menu.show {
		font-size: 14px !important ;
	}
	.bg-black {
		font-size: 14px;
	}
}

@media (min-width: 1400px) {
	.dpd-button {
		gap: 100px;
	}
	button {
		font-size: 16px;
	}
	.dropdown-menu.show {
		font-size: 16px !important ;
	}
	.bg-black {
		font-size: 16px;
	}
}

@media (min-width: 1700px) {
	.dpd-button {
		gap: 150px;
	}
}
</style>
