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
    <h1 :class="{ change:color }"> Third Component {{ msg }}</h1>
    <button v-on:click="color=!color">change info</button>

</template>
<script> 
export default {
    data() {
        return {       
            color:false     
        }
    },
    methods: {

    }
}
</script>

<style>
.change{
    color: wheat;
}
</style>