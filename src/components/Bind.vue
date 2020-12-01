<template>
    <div class="form">
    {{ note }}
        <input type="text" v-model='note'>
    </div>
</template>
<script>
export default {
    name: "Bind",
    data(){
        return {
            note:"Hi"
        }
    }
}
</script>