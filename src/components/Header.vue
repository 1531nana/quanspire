<template>
	<nav
		class="navbar navbar-expand-lg navbar-dark"
		style="background-color: black"
	>
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
				<li class="nav-item active">
					<a class="nav-link" href="#">Overview</a>
				</li>
				<li class="nav-item">
					<a class="nav-link active" href="#">Data Model</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#">Analytics</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#">Markets</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#">Optimizer</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#">Hedge</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#">Trader</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#">Supervisor</a>
				</li>
			</ul>
		</div>
		<div class="d-flex gap-3 align-items-center">
			<div>
				<div class="d-flex rounded-pill bg-dark flex-row currencies">
					<div
						class="btn btn-primary rounded-pill border-0 d-flex align-items-center interruptor"
						type="button"
						style="background: #2c4190"
					>
						Currencies
					</div>
					<div
						class="btn btn-dark rounded-pill border-0 d-flex align-items-center interruptor"
						type="button"
						style="color: #ffffff8c"
					>
						Commodities
					</div>
				</div>
			</div>
			<div class="d-flex flex-row gap-2 p-3 border-1 border-start border-end">
				<div class="d-flex align-items-baseline gap-1">
					<p class="m-0" style="color: #ffffff8c">Iván Herrera</p>
					<img src="../assets/fa_user.svg" alt="user" />
				</div>
				<div class="d-flex currencies rounded-pill bg-dark">
					<div
						class="btn btn-dark rounded-pill border-0 d-flex align-items-center"
						style="color: #ffffff8c"
					>
						Light
					</div>
					<div
						class="btn btn-primary rounded-pill border-0 d-flex align-items-center"
						style="background: #2c4190"
					>
						Dark
					</div>
				</div>
			</div>
			<img src="../assets/off.png" alt="" class="off" />
		</div>
	</nav>
</template>

<style scoped>
.navbar-expand-lg .navbar-nav {
	border-left: 1px solid;
}
 .navbar-dark {
	box-shadow: -1px 1px 5px grey !important;
	z-index: 1 !important;
}

.currencies {
	height: 25px;
}
.interruptor {
	height: 100%;
}
.off {
	padding-right: 1rem;
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
	.navbar-dark {
		font-size: 12px !important;
	}
	.gap-3 {
		gap: 0.5rem !important;
	}
	.currencies {
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
	.navbar-expand-lg .navbar-nav {
		padding-left: 5px !important;
	}
	.navbar-expand-lg .navbar-nav .nav-link {
		padding: 5px !important;
	}

	.navbar-dark {
		font-size: 14px !important;
	}
	.gap-3 {
		gap: 0.5rem !important;
	}
	.currencies {
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
	.navbar-dark {
		font-size: 16px !important;
	}
	.navbar-dark {
		font-size: 16px !important;
	}
	.currencies {
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
