<script setup>
defineProps({
}
)
</script>
<template>
    <h1> Watchers </h1>
   <h4>{{ count }}</h4>
    <button v-on:click="count++" >+</button>
    <button v-on:click="count--" >-</button>

    
   
</template>
<script>
export default {
    data() {
        return {
           count:0
        }
    },
    watch:{
        count(value)
        {
            if(value>5)
            {
                alert("stop")
            }
        }
    }
}
</script>