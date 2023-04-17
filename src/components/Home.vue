<script setup>
defineProps({
    msg: {
        type: String,
        required: true
    }
}
)
</script>
<template>
    <h1>{{ getname("M Daniyal") }} </h1>
    <h1>{{ email }}</h1>
    <h1>{{ mob }}</h1>
    <h1>{{ mob==50 }}</h1>
</template>
<script>
export default {
    data() {
        return {
            email: 'admin@gmail.com',
            mob:'202',
        }
    },
    methods:{
        getname(name){
            return name;
        }
    }
}
</script>