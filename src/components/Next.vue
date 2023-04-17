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
    <h1>Check Boxes and Radio Buttons</h1>
    <label for="abc">ABC</label>
    <input type="checkbox" name="abc" id="abc" value="abc" v-model="tech"/> <br>
    <label for="xyz">XYZ</label>
    <input type="checkbox" name="xyz" id="xyz" value="xyz" v-model="tech"/>
    <br><br>
    <label for="male">Male</label>
    <input type="radio" name="who" id="male" value="male" v-model="who"/>

    <label for="woman">Woman</label>
    <input type="radio" name="who" id="woman" value="woman" v-model="who"/>

    <h4>Selected Checkboxes: {{ tech }}</h4>
    <h4>Selected Radio: {{ who }}</h4>
</template>
<script>
export default {
    data() {
        return {
           tech:[],
           who:null
        }
    },
    methods:{
       
    }
}
</script>