<script setup>
defineProps({
    msg:{type:String}
}
)
</script>
<template>
    <h1> Slot Practice </h1>
    <slot name="header"></slot>
    
   
   
</template>
<script>
export default {
    data() {
        return {
        }
    },
  
}
</script>