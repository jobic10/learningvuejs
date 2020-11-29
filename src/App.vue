<template>
<div class="body">
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <Home data="We are thrilled to have you visit us"/>
  <Users/>
  <products></products>
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
  }
}
</script>
<style scoped>
.body{
background-color: #70dab6;
height: 1000px;
}
</style>

