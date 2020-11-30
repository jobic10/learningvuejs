<template>
    <div class="child">
        <h1 v-bind:style="{color:colorName}">Products</h1>
        <p v-bind:class="{display:show}">Our products...</p>
    </div>
</template>
<script>
export default {
    name: "Products",
    data(){
        return {
            colorName:'magenta',
            show:true
        }
    }
}
</script>

<style scoped>
.child{
    background-color: rgb(145, 121, 91);
    height: auto;
    width: auto;
    padding: 30px;
    margin: 20px;
}
.display{
    background-color: darkslategray;
}
</style>