<template>
	<div class="d-flex bg-darks">
		<div class="bd-search" id="docsearch" data-bd-docs-version="5.2">
			<input type="text" placeholder="Keyword Search" class="input-search" />
			<svg
				width="20"
				height="20"
				class="search-Icon position-absolute"
				viewBox="0 0 20 20"
			>
				<path
					d="M14.386 14.386l4.0877 4.0877-4.0877-4.0877c-2.9418 2.9419-7.7115 2.9419-10.6533 0-2.9419-2.9418-2.9419-7.7115 0-10.6533 2.9418-2.9419 7.7115-2.9419 10.6533 0 2.9419 2.9418 2.9419 7.7115 0 10.6533z"
					stroke="currentColor"
					fill="none"
					fill-rule="evenodd"
					stroke-linecap="round"
					stroke-linejoin="round"
				></path>
			</svg>
		</div>
		<div class="container-actions">
			<span class="actions">
				<span>+</span>
				Fields
				<div class="container-switch">
					<input
						class="check-input"
						type="checkbox"
						role="switch"
						id="btn-switch"
					/>
					<label for="btn-switch" class="lbl-switch"></label>
				</div>
			</span>
			<span v-for="(action, i) in actions" :key="i" class="actions">
				{{ action }}
				<img :src="getImages(imagesName[i])" :alt="imagesName[i]" class="img-actions" />
			</span>
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			actions: ["Download:", "Upload:", "Add:", "Saved:", "Synced:", "Delete:"],
			imagesName: ["download", "upload", "plus", "saved", "saved", "delet"],
		};
	},
	methods: {
		getImages(urlImg) {
			return require("..\/assets\/" + urlImg + ".svg");
		},
	},
};
</script>

<style scoped>
.bg-darks {
	background: #232227;
	padding: 15px;
}
.d-flex {
	gap: 30px;
}
.bd-search {
	display: flex;
	height: 100%;
	position: relative;
}
.search-Icon {
	bottom: 30%;
	left: 5%;
}
.input-search {
	text-align: center;
	background: #0f0e13;
	border: none;
	border-radius: 5px;
	padding: 8px;
	width: 250px;
	box-shadow: 0 1px #ffffff8f;
}
.actions {
	display: flex;
	justify-content: center;
	align-items: center;
	gap: 5px;
}

.lbl-switch {
	display: flex;
	align-items: center;
	width: 40px;
	height: 20px;
	background: #ffffff8f;
	border-radius: 100px;
	position: relative;
	cursor: pointer;
}
#btn-switch:checked ~ .lbl-switch {
	background: #2c4190;
}

.lbl-switch:after {
	position: absolute;
	content: "";
	width: 25px;
	height: 25px;
	border: 1px solid #ffffff8f;
	background: black;
	border-radius: 100px;
	left: 0;
	transition: 0.3s;
}
#btn-switch:checked ~ .lbl-switch:after {
	left: 25px;
}
#btn-switch {
	display: none;
}
.container-actions {
	display: flex;
	width: 100%;
	justify-content: space-around;
}

@media (min-width: 1280px) {
	.d-flex {
		gap: 60px;
	}
	.img-actions {
		width: 20px;
	}
}

@media (min-width: 1400px) {
	.d-flex {
		gap: 75px;
	}
	.img-actions {
		width: 22px;
	}
}
</style>
