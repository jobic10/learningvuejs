<template>
    <div>
        <button v-on:click="updateTitle()">Update title</button>
    </div>
</template>
<script>
export default {
    name: "Child",
    methods: {
        updateTitle(){
            this.$emit('change-title', 'Child Props Has Been Passed!')
        }
    }
}
</script>