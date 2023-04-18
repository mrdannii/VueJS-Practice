<script setup>
defineProps({
}
)
</script>
<template>
    <h1> FORM Component </h1>
    <p>{{ form }}</p><br><br>
    <ul>
        <li v-for="item in error" v-bind:key="item">{{ item }} Not Valid</li>
    </ul>

    
    <form action="">
        <label for="email">Email : </label>
        <input type="email" name="email" id="email" v-model.lazy="form.email">
        <br>
        <label for="password">Password : </label>
        <input type="password" name="password" id="password" v-model="form.pass">
        <br>
        <button type="button" v-on:click="login()">Submit</button>
        <input type="text" name="a" id="a" v-model="form.a">
        <input type="text" name="b" id="b" v-model="form.b">
        <input type="text" name="c" id="c" v-model="form.c">

    </form>
</template>
<script>
export default {
    data() {
        return {
            form: {
                email: '', pass: '', a:'', b:'', c:'',
            },
            error: []
        }
    },
    methods: {
        login() {
             this.error = [];
            for (const item in this.form) {
                if(this.form[item]==="" || this.form[item].length===0){
                    this.error.push(item)
                }
            }

            if(this.error.length===0)
            {
                alert("Form Submitted")

            }
        }
    }
}
</script>