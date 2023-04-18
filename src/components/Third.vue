<script setup>
    import Next from './Next.vue'

    defineProps({
        msg: {
            type: String,
            required: true
        }
    }
    )


    </script>
<template>
    <h1> Third Component {{ msg }}</h1>
    <Next/>
    
</template>
<script> 
export default {
    data() {
        return {            
        }
    },
    methods: {

    }
}
</script>