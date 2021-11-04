<template>
    <h1>hello, world!</h1>

	<Table
		:columns="['name', 'last_name']"
		:data="[
			{ name: 'Ayax', last_name: 'Córdova' },
			{ name: 'Eunice', last_name: 'Ramos' },
		]"
	/>
</template>

<script>
import Table from './components/Table.vue';
export default {
    name: "App",
    components: { Table },
};
</script>

<style></style>
