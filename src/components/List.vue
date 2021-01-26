<template>
    <div class="container">
        <b-card :title="element.title" v-for="(element) in elements" :key="element.id">
            <b-card-text>{{element.description}}</b-card-text>
        </b-card>
    </div>
</template>

<script>
export default {
    name: 'List',
    created() {
        this.getAll()
    },
    data() {
        return {
            elements: [],
        }
    },
    methods: {
        getAll() {
            fetch('http://127.0.0.1:8000/api/element/?format=json')
            .then(res => res.json())
            .then(res => this.elements = res)
        }
    },
}
</script>

<style>

</style>