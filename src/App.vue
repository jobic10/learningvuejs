<template>
<div class="body">
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <Home data="We are thrilled to have you visit us"/>
  <Users/>
  <products></products>
  <h1 v-once>{{ name }}</h1>
  <h1>{{ name }}</h1>
  <button v-on:click="func()">Click</button>
</div>
</template>

<script>
import Home from './components/Home'
import Users from '@/components/Users'
import Products from './components/Products.vue'
export default {
  name: 'App',
  components: {
    Home,
    Users,
    Products
  },
  data() {
    return {
      name: "Job"
    }
  },
  methods: {
    func(){
      this.name = "Owonubi Job Sunday"
    }
  },
}
</script>
<style scoped>
.body{
background-color: #70dab6;
height: 1000px;
}
</style>

