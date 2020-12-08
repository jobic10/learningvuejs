<template>
<div class="body">
  <child v-on:change-title="updateText($event)" />
  <h1 v-once>{{ name }}</h1>
  <h1>{{ name }}</h1>
  <button v-on:click="func()">Click</button>
  <h4>{{ isValid? "Yes":"No" }}</h4>
</div>
</template>

<script>
import Child from '@/components/Child'
export default {
  name: 'App',
  components: {
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
      beforeUpdate: function() {
        alert('Before Updated')
    },
    updated: function(){
        alert('updated')
    }
}
</script>
<style scoped>
.body{
background-color: #70dab6;
height: 1000px;
}
</style>

