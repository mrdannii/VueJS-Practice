<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Home from './components/Home.vue'
import Next from './components/Next.vue'
import Second from './components/Second.vue'
import Third from './components/Third.vue'
import Child from './components/child.vue'
import Form from './components/Form.vue'

</script>

<template>
  <header>
    <!-- <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" /> -->

    <div class="wrapper">
      <!-- <HelloWorld msg="VueJS Practice " /> -->
      <!-- <button v-on:click="show = !show"> Third</button> -->

    </div>
  </header>

  <main>
    <!-- <Home msg="Daniyal"/> -->
    <!-- <Next/> -->
    <!-- <Second /> -->
    <!-- <Third v-if="show" msg="hehe"/> -->
    <!-- <Child :get-usern="getUserN" /> -->
    <Form />

  </main>
</template>

<script>
export default {
  data() {
    return {
      show: true,

    }
  },
  methods: {
    getUserN(uam) {
      alert(uam)
    }
  }
}
</script>
<!-- <style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style> -->
