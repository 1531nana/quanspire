<template>
	<td>
		<div class="d-flex">
			<img
				v-for="(imageName, i) in imagesNames"
				:key="i"
				:src="getImage(imageName)"
				:alt="imageName"
			/>
		</div>
	</td>
</template>

<script>
export default {
	data(){
		return{
			imagesNames:  ['pencil', 'copy', 'delete']
		}
	},
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
