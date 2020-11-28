<template>
    <div>
        <h1>Hello From Home View</h1>
        <h4>{{ data }}</h4>
    </div>
</template>
<script>
export default {
    name: 'Home',
    props:{
        data:String
    }
}
</script>