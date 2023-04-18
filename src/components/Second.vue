<!-- <script setup>
    defineProps({
        msg: {
            type: String,
            required: true
        }
    }
    )
    </script> -->
<template>
    <h1 v-if="show"> if conditon</h1>
    <h1 v-else> else conditon</h1>
    <button v-on:click="show = !show"> Toggle</button>

    <ul>
        <li v-for="item in tech">{{ item }}</li>
    </ul>

    <ul>
        <li v-for="item in user">Name : {{ item.name }} <br> Gender: {{ item.gender }}</li>
    </ul>
</template>
<script> 
export default {
    data() {
        return {
            show: true,
            tech: ['java', 'php', 'c++'],
            user: [
                { name: "dani", gender: 'male' },
                { name: "emily", gender: 'women' }
            ],
        }
    },
    methods: {

    }
}
</script>