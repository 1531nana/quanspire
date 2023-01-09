<template>
	<tr>
		<td colspan="9">
			<ul class="pagination">
				<li class="page-item">
					<a class="page-link" href="#" aria-label="Previous">
						<span aria-hidden="true">&laquo;</span>
					</a>
				</li>
				<li class="page-item">
					<a class="page-link" href="#" aria-label="Next">
						<span aria-hidden="true">‹</span>
					</a>
				</li>
				<li class="page-item"><a class="page-link active" href="#">1</a></li>
				<li class="page-item"><a class="page-link" href="#">2</a></li>
				<li class="page-item"><a class="page-link" href="#">3</a></li>
				<li class="page-item"><a class="page-link" href="#">4</a></li>
				<li class="page-item"><a class="page-link" href="#">5</a></li>
				<li class="page-item">
					<a class="page-link" href="#" aria-label="Next">
						<span aria-hidden="true">›</span>
					</a>
				</li>
				<li class="page-item">
					<a class="page-link" href="#" aria-label="Next">
						<span aria-hidden="true">&raquo;</span>
					</a>
				</li>
			</ul>
		</td>
		<td colspan="2" class="show">
			<label for="" class="show-pages">Showing 1 to 15 of 145 entries</label>
			<button
				class="btn btn-dark dpd-button"
				type="button"
				data-bs-toggle="dropdown"
				aria-expanded="false"
			>
				15 <img src="../../assets/select.svg" alt="" />
			</button>
			<ul class="dropdown-menu">
				<li><a class="dropdown-item" href="#">30</a></li>
			</ul>
		</td>
	</tr>
</template>

<style scoped>
.show {
	padding: 0;
	border: none;
}
.show-pages {
	color: #ffffff5e;
	font-size: 8px;
}
.dpd-button {
	font-size: 10px;
	margin-left: 10px;
	background: rgba(0, 0, 0, 0);
	border: none;
	border-bottom: 1px solid #ffffff5e;
	border-radius: 0;
	padding-bottom: 2px;
}
img {
	width: 6px;
	margin-left: 10px;
}
.page-link {
	border: none !important;
	background: rgb(0, 0, 0, 0);
	color: #ffffff5e;
	font-size: 12px;
}
.active > .page-link,
.page-link.active {
	background: #ffffff5e;
	border-radius: 5px;
}
@media (min-width: 1280px) {
	.show-pages {
		font-size: 10px;
	}
	.dpd-button {
		font-size: 12px;
	}
	.page-link {
		font-size: 14px;
	}
	img {
		width: 8px;
	}
	.pagination {
		gap: 2px;
	}
}
@media (min-width: 1400px) {
	.show-pages {
		font-size: 12px;
	}
	.dpd-button {
		font-size: 14px;
	}
	.page-link {
		font-size: 16px;
	}
	img {
		width: 10px;
	}
	.pagination {
		gap: 5px;
	}
}
@media (min-width: 1500px) {
	.show-pages {
		font-size: 14px;
	}
	.dpd-button {
		font-size: 14px;
	}
	.page-link {
		font-size: 16px;
	}
	img {
		width: 10px;
	}
	.pagination {
		gap: 8px;
	}
}
@media (min-width: 1700px) {
  	.show-pages {
		font-size: 16px;
	}
	.dpd-button {
		font-size: 18px;
	}
	.page-link {
		font-size: 20px;
	}
	img {
		width: 14px;
	}
	.pagination {
		gap: 10px;
	}
}
@media (min-width: 1800px) {
  .pagination{
    gap: 13px;
  }
}

</style>
