<script setup>
    defineProps({
        msg: {
            type: String,
            required: true
        },
        getUsern:{type:Function, required:true},
    }
    )
    </script>
<template>
    <h1 > Child Component </h1>
   <button v-on:click="getUsern(uname)">Send Nanme</button>
   
</template>
<script> 
export default {
    data() {
        return {
           uname:"SAM"
        }
    },
    methods: {

    }
}
</script>