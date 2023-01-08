<template>
	<div class="dropdown bg-black">
		<span>CREATE/UPDATE: <img src="../assets/update.svg" alt="" /></span>
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
			<li><a class="dropdown-item" href="#">EUR</a></li>
			<li><a class="dropdown-item" href="#">YEN</a></li>
			<li><a class="dropdown-item" href="#">PEN</a></li>
			<li><a class="dropdown-item" href="#">MXN</a></li>
			<li><a class="dropdown-item" href="#">Corn</a></li>
			<li><a class="dropdown-item" href="#">Soya</a></li>
		</ul>
	</div>
</template>

<style scoped>
.bg-black {
	font-size: 12px;
	display: flex;
	gap: 25px;
	align-items: center;
	padding-left: 5px;
  padding: 10px;
}
.dpd-button {
	width: 15%;
	display: flex;
	justify-content: space-between;
	align-items: center;
	background: #6c757d36 !important;
	border-radius: 0 !important;
	padding: 5px !important;
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
