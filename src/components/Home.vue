<template>
    <div class="home">
        <h1 align='center'>Welcome To Our Official Website</h1>
        <h4>{{ data }}</h4>
        <button v-on:click="toggleDisplay()">Toggle</button>
        <h1 v-if="show">Lights On</h1>
        <h1 v-else>Lights Out</h1>
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
}
</script>
