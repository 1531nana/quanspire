<template>
	<td>
		<div class="d-flex">
			<img
				v-for="(im, i) in ['pencil', 'copy', 'delete']"
				:key="i"
				:src="getImage(im)"
				:alt="im"
			/>
		</div>
	</td>
</template>

<script>
export default {
	methods: {
		getImage(image) {
			return require("..\/..\/assets\/" + image + ".svg");
		},
	},
};
</script>

<style scoped>
.d-flex {
	justify-content: space-around;
}
img {
	width: 15px;
}
@media (min-width: 1280px) {
	img {
		width: 16px;
	}
}
@media (min-width: 1500px) {
	.d-flex {
		justify-content: space-evenly;
	}
}
</style>
