<template>
    <table>
        <thead>
            <tr v-if="columns.length">
                <th>Actions</th>
                <th v-for="col of columns" :key="col">{{ col }}</th>
            </tr>
        </thead>

        <!-- Data v-for -->
        <tbody>
            <tr v-for="row of data" :key="row.id">
                <td>
                    Actions
                    <button>lorem 1</button>
                    <button>lorem 2</button>
                </td>

                <td v-for="(value, key) of row" :key="key">{{ value }}</td>
            </tr>
        </tbody>
    </table>
</template>

<script>
export default {
    props: {
        columns: {
            type: Array,
            required: true,
        },
        data: {
            type: Object,
            require: true,
            default: () => {},
        }
    },

    components: {},

    setup () {

        return {
        }
    }
}
</script>

<style lang="scss" scoped>

</style>