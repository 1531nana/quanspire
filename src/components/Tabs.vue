<template>
	<ul class="nav nav-tabs">
		<li class="nav-item">
			<a class="nav-link active" aria-current="page" href="#">EXPOSURES</a>
		</li>
		<li class="nav-item">
			<a class="nav-link" href="#">HEDGES</a>
		</li>
		<li class="nav-item">
			<a class="nav-link" href="#">PROGRAM</a>
		</li>
	</ul>
</template>

<style scoped>
.containerTabs {
	position: fixed;
	bottom: 0;
	width: 100%;
	height: 100%;
}
.nav-tabs {
	width: 45%;
	border: none;
	position: absolute;
	bottom: 0;
}
.nav-item {
	width: 33%;
	background: #232227;
	border-radius: 0 10px 0 0 !important;
	border: 1px solid #636967 !important;
}
.nav-link {
	padding: 0;
	color: #636967;
	font-size: 14px;
}
.nav-tabs .nav-item.show .nav-link,
.nav-tabs .nav-link.active {
	background: #0b2b8c;
	color: white;
	border-radius: 0 10px 0 0 !important;
	border: none;
}
</style>
