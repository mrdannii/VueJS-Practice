<script setup>
import Form from './Form.vue'
import Next from './Next.vue'
import Third from './Third.vue'

import Footer from './Footer.vue'

</script>
<template>
    <h1> Dynamic components </h1>
  <button @click="tab='Form'">form </button>
  <button @click="tab='Next'">next </button>
  <button @click="tab='Third'"> third</button>

    <component :is="tab"/>

    <Teleport to="#footer">
        <Footer/>
    </Teleport>
   
</template>
<script>
export default {
    data() {
        return {
            tab:''
        }
    },
    components:{
        Form,Third,Next
    }
   
}
</script>