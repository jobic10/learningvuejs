<template>
<div class="body">
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <Home data="We are thrilled to have you visit us"/> -->
  <child v-on:change-title="updateText($event)" />
  <!-- <bind/> -->
  <!-- <Users/> -->
  <!-- <products></products> -->
  <h1 v-once>{{ name }}</h1>
  <h1>{{ name }}</h1>
  <button v-on:click="func()">Click</button>
  <h4>{{ isValid? "Yes":"No" }}</h4>
</div>
</template>

<script>
// import Home from './components/Home'
// import Users from '@/components/Users'
// import Products from './components/Products.vue'
// import Bind from '@/components/Bind'
import Child from '@/components/Child'
export default {
  name: 'App',
  components: {
    // Home,
    // Users,
    // Products,
    // Bind,
    Child
  },
  data() {
    return {
      name: "Child to parent Data",
      'isValid': false
    }
  },
  methods: {
    func(){
      this.name = "Owonubi Job Sunday"
    },
    updateText(title){
    this.name = title
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

