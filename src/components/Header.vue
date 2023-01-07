<template>
	<nav
		class="navbar navbar-expand-lg navbar-dark bg-dark"
		style="background-color: black"
	>
		<a class="navbar-brand" href="#"
			><img src="../assets/Quanspire.png" alt=""
		/></a>
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
				<div>
					<div class="nav-link">Currencias</div>
					<div class="nav-link">Commodities</div>
				</div>
                <div>
                    <p class="nav-link">Iván Herrera</p>
                    <img src="../assets/users.png" alt="" style="height: 10px"/>
                </div>
				<div>
					<div class="nav-link">Light</div>
					<div class="nav-link">Dark</div>
				</div>
			</ul>
		</div>
                    <img src="../assets/off.png" alt="" />
	</nav>
</template>


<style>
#app .bg-dark{
    background: black !important;
}
</style>
