<template>
	<tr v-for="(data, i) in datas" :key="i" style="background: rgb(0 0 0 / 78%) !important">
		<TableBodyActions />
		<td>{{ `Q2460${index - 1}` }}</td>
		<td>{{ datas[i].portfolio }}</td>
		<td>{{ data.rate }}</td>
		<td>{{ data.exposure }}</td>
		<td>{{ data.notional }}</td>
		<td>{{ data.currency }}</td>
		<td>{{ expDate[index - 1] }}</td>
		<td>{{ data.issueDate }}</td>
		<td>{{ data.rateDate }}</td>
		<td>{{ data.invoiceDate }}</td>
	</tr>
</template>

<script>
import TableBodyActions from "./TableBodyActions.vue";

export default {
	props: {
		index: Number,
	},
	data() {
		return {
			datas: [
				{
					portfolio: "1YLAYERS",
					rate: "USDCOP",
					exposure: "PROJECTED COSTS",
					notional: "1,000,000",
					currency: "USD",
					issueDate: "-",
					rateDate: "-",
					invoiceDate: "-",
				},
			],
			expDate: [
				"15 Jan 10",
				" 15 Feb 10",
				"15 Mar 10",
				"15 Apr 10",
				"15 May 10",
				"15 Sep 10",
				"15 Oct 10",
				"15 Nov 10",
				"15 Dec 10",
				"15 Jan 11",
				"15 Feb 11",
			],
		};
	},

	components: {
		TableBodyActions,
	},
};
</script>
