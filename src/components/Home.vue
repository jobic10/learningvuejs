<template>
    <div>
        <h1>Hello From Home View</h1>
        <h4>{{ data }}</h4>
        <button v-on:click="hello()">Call</button>
    </div>
</template>
<script>
export default {
    name: 'Home',
    props:{
        data:String
    },
    methods: {
        hello(){
            alert("Hello Function Called")
        }
    }
}
</script>