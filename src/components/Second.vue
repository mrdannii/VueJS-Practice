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
       <h1 v-if="show"> if conditon</h1>
       <h1 v-else> else conditon</h1>

       <button v-on:click="show=!show"> Toggle</button>
    </template>
    <script>
    export default {
        data() {
            return {
               show:true
            }
        },
        methods:{
           
        }
    }
    </script>