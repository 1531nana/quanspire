<template>
	<div class="dropdown bg-black">
		<span
			>CREATE/UPDATE: <img src="../assets/update.svg" alt="" class="update"
		/></span>
		<label for="">COMPANY:</label>
		<button
			class="btn btn-secondary dpd-button"
			type="button"
			data-bs-toggle="dropdown"
			aria-expanded="false"
		>
			QUANSPIRE <img src="../assets/select.svg" alt="" />
		</button>
		<ul class="dropdown-menu">
			<li><a class="dropdown-item" href="#">SURA</a></li>
			<li><a class="dropdown-item" href="#">Challenger</a></li>
			<li><a class="dropdown-item" href="#">Acepalma</a></li>
		</ul>
		<label for="">PORTFOLIOS:</label>
		<button
			class="btn btn-secondary dpd-button"
			type="button"
			data-bs-toggle="dropdown"
			aria-expanded="false"
		>
			1YLAYERS <img src="../assets/select.svg" alt="" />
		</button>
		<ul class="dropdown-menu">
			<li><a class="dropdown-item" href="#">2YLAYERS</a></li>
		</ul>
		<label for="">CURRENCIES:</label>
		<button
			class="btn btn-secondary dpd-button"
			type="button"
			data-bs-toggle="dropdown"
			aria-expanded="false"
		>
			USDCOP <img src="../assets/select.svg" alt="" />
		</button>
		<ul class="dropdown-menu">
			<li v-for="(currencie, i) in currencies" :key="i">
				<a class="dropdown-item" href="#">{{ currencie }}</a>
			</li>
		</ul>
	</div>
</template>

<script>
export default {
	data() {
		return {
			currencies: ["EUR", "YEN", "PEN", "MXN", "Corn", "Soya"],
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
	width: 15%;
	display: flex;
	justify-content: space-between;
	align-items: center;
	background: #0f0e13 !important;
	border-radius: 0 !important;
	padding: 5px 10px !important;
	border-width: 0 0 2px 0;
}
button {
	font-size: 12px;
}
.dropdown-menu.show {
	font-size: 12px !important ;
}

@media (min-width: 1280px) {
	.dpd-button {
		width: 16%;
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
		width: 16%;
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
</style>
