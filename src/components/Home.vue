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
    <h1 v-on:mouseover="mouse()">{{ getname() }}  </h1><h2>{{ count }}</h2> 
    <h1>{{ email }}</h1>
    <h1>{{ mob }}</h1>
    <h1>{{ mob==50 }}</h1>
    <button v-on:click="test('button')">Click</button>
    <button v-on:dblclick="test('button double')"> 2 Click</button><br>
    <input type="text" v-model="inputtext"><p><strong> {{ inputtext }}</strong></p>

    <input type="text" name="" id="" placeholder="text" v-model="text">
    <input type="email" name="" id="" placeholder="email" v-model="email2">
    <button v-on:click="getinputdata()"> Get Data</button>


</template>
<script>
export default {
    data() {
        return {
            name:"Dannii",
            email: 'admin@gmail.com',
            mob:'202',
            count:0,
            inputtext:"",
            text:null,
            email2:null,
        }
    },
    methods:{
        getinputdata(){
            alert("Text: " +this.text + " And Email: " +  this.email2)
        },
        getname(){
            return this.name;
        },
        test(data){
            alert(data)
        },
        mouse(){
            this.count++;
        }
    }
}
</script>