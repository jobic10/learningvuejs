<template>
    <div>
        <h1>Hello From Home View</h1>
        <h4>{{ data }}</h4>
        <button v-on:click="toggleDisplay()">Toggle</button>
        <h1 v-if="show">True</h1>
        <h1 v-else> False</h1>

    </div>
</template>
<script>
export default {
    name: 'Home',
    props:{
        data:String
    },
    methods: {
        toggleDisplay(){
            this.show = !this.show
        }
    },
    data(){
        return{
            show:false
        }
    }
}
</script>