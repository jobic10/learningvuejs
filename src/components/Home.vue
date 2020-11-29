<template>
    <div>
        <h1>Hello From Home View</h1>
        <h4>{{ data }}</h4>
        <button v-on:click="hello('Job')">Call</button>
    </div>
</template>
<script>
export default {
    name: 'Home',
    props:{
        data:String
    },
    methods: {
        hello(name){
            alert("Hello " + name)
        }
    }
}
</script>