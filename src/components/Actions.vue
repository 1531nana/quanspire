<template>
	<div class="d-flex bg-dark">
		<div class="bd-search" id="docsearch" data-bd-docs-version="5.2">
			<input type="text" placeholder="Keyword Search" class="input-search" />
			<svg
				width="20"
				height="20"
				class="DocSearch-Search-Icon position-absolute"
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
		<div class="d-flex">
			<span class="actions">
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
			<span class="actions"
				>Download
				<img src="../assets/download.svg" alt="" class="img-actions" />
			</span>
			<span class="actions"
				>Upload <img src="../assets/upload.svg" alt="" class="img-actions" />
			</span>
			<span class="actions"
				>Add <img src="../assets/plus.svg" alt="" class="img-actions" />
			</span>
			<span class="actions"
				>Saved <img src="../assets/saved.svg" alt="" class="img-actions" />
			</span>
			<span class="actions"
				>Synced <img src="../assets/saved.svg" alt="" class="img-actions" />
			</span>
			<span class="actions"
				>Delete <img src="../assets/delete.svg" alt="" class="img-actions" />
			</span>
		</div>
	</div>
</template>

<style scoped>
.bg-dark {
	padding: 15px;
}
.d-flex {
	gap: 30px;
}
.bd-search {
	display: flex;
	width: 100%;
	height: 100%;
	position: relative;
}
.DocSearch-Search-Icon {
	bottom: 20%;
	left: 5%;
}
.input-search {
	text-align: center;
	background: #0000009e;
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
.img-actions {
	width: 16px;
}
.lbl-switch{
    /* display: inline-block; */
    display: flex;
    align-items: center;
    width: 40px;
    height: 20px;
    background: #ffffffc8;
    border-radius: 100px;
    position: relative;
    cursor: pointer;
}
#btn-switch:checked~ .lbl-switch{
    background: #2c4190;
}

.lbl-switch:after{
position: absolute;
content: '';
width: 25px;
height: 25px;
border: 1px solid #ffffffc8;
background: black;
border-radius: 100px;
left: 0;
transition: 0.3s;
}
#btn-switch:checked~ .lbl-switch:after{
    left: 25px;
}
#btn-switch{
    display: none;
}
</style>
