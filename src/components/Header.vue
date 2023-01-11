<template>
	<nav class="navbar navbar-expand-lg navbar">
		<a class="navbar-brand" href="#">
			<img src="../assets/Quanspire.png" alt="" class="logo" />
		</a>
		<button
			class="navbar-toggler"
			type="button"
			data-toggle="collapse"
			data-target="#navbarNav"
			aria-controls="navbarNav"
			aria-expanded="false"
			aria-label="Toggle navigation"
		>
			<span class="navbar-toggler-icon"></span>
		</button>
		<div class="collapse navbar-collapse" id="navbarNav">
			<ul class="navbar-nav">
				<li v-for="(itemNav, i) in itemsNav" :key="i" class="nav-item">
					<a class="nav-link" :class="{ 'active': i == 1}" href="#" >{{ itemNav }}</a>
				</li>
      </ul>
		</div>
		<div class="d-flex gap-3 align-items-center">
				<div class="d-flex rounded-pill bg-dark flex-row container-btns">
					<div
						class="btn btn-primary rounded-pill border-0 d-flex align-items-center btns-c btns-active"
						type="button"
					>
						Currencies
					</div>
					<div
						class="btn btn-dark rounded-pill border-0 d-flex align-items-center btns-c"
						type="button"
					>
						Commodities
					</div>
			</div>
			<div class="d-flex flex-row gap-2 p-3 border-1 border-start border-end">
				<div class="d-flex align-items-baseline gap-1">
					<p class="m-0">Iván Herrera</p>
					<img src="../assets/fa_user.svg" alt="user" class="user" />
				</div>
				<div class="d-flex container-btns rounded-pill bg-dark">
					<div
						class="btn btn-dark rounded-pill border-0 d-flex align-items-center"
					>
						Light
					</div>
					<div
						class="btn btn-primary rounded-pill border-0 d-flex align-items-center btns-active"
					>
						Dark
					</div>
				</div>
			</div>
			<img src="../assets/off.png" alt="" class="off" />
		</div>
	</nav>
</template>

<script>
export default {
	data() {
		return {
			itemsNav: [
				"Overview",
				"Data Model",
				"Analytics",
				"Markets",
				"Optimizer",
				"Hedge",
				"Trader",
				"Supervisor",
			],
		};
	},
};
</script>

<style scoped>
.user {
	width: 8px;
}
.nav-link,
.d-flex {
	color: #ffffff8f !important;
}
.navbar-nav .nav-link.active,
.navbar-nav .show > .nav-link {
	color: white !important;
}
.btns-active {
	background: #2c4190;
	color: white !important;
}
.navbar-expand-lg .navbar-nav {
	border-left: 1px solid #ffffff4d;
	height: 36px;
	align-items: center;
	justify-content: space-between;
}
.navbar {
	box-shadow: 1px 3px 2px 0px #80808069 !important;
	z-index: 1 !important;
}

.container-btns {
	height: 25px;
}
.btns-c {
	height: 100%;
}
.off {
	padding-right: 1rem;
	width: 18px;
	margin-right: 5px;
}
.border-start,
.border-end {
	border-left: 1px solid #ffffff4d !important ;
	border-right: 1px solid #ffffff4d !important ;
}
.navbar-expand-lg .navbar-nav {
	padding-left: 5px !important;
}

@media (min-width: 1024px) {
	.navbar-brand {
		margin-right: 0 !important;
	}
	.logo {
		width: 150px;
	}
	.navbar-expand-lg .navbar-nav .nav-link {
		padding: 4px !important;
	}
	.navbar {
		font-size: 12px !important;
	}
	.gap-3 {
		gap: 0.5rem !important;
	}
	.container-btns {
		height: 20px !important;
	}
	.btn {
		font-size: 12px !important;
	}
	.p-3 {
		padding: 0.5rem !important;
	}
	.off {
		padding-right: 0.25rem !important;
	}
}

@media (min-width: 1280px) {
	.navbar-brand {
		margin-right: 0 !important;
	}
	.logo {
		width: 200px;
	}

	.navbar-expand-lg .navbar-nav .nav-link {
		padding: 5px !important;
	}

	.navbar {
		font-size: 14px !important;
	}
	.gap-3 {
		gap: 0.5rem !important;
	}
	.container-btns {
		height: 20px !important;
	}
	.btn {
		font-size: 14px !important;
	}
	.p-3 {
		padding: 0.5rem;
	}
}

@media (min-width: 1400px) {
	.navbar {
		font-size: 16px !important;
	}
	.navbar {
		font-size: 16px !important;
	}
	.container-btns {
		height: 25px !important;
	}
	.btn {
		font-size: 16px !important;
	}
	.p-3 {
		padding: 1rem !important;
	}
}
</style>
