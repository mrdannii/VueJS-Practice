<script setup>
import axios from 'axios'

</script>
<template>
    <h1> Data From Api </h1>
    <ul>
        <li v-for="item in data" >{{ item.id }} ---{{ item.first_name }} --- {{ item.email }} --- <img height="50" width="50" :src="item.avatar" /> </li>
    </ul>
   
</template>
<script>
export default {
    data() {
        return {
            data:[]
        }
    },
    async mounted()
    {
        let res=await axios.get("https://reqres.in/api/users?page=1");
        this.data=res.data.data;
    }
   
}
</script>