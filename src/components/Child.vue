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
    },
    beforeCreate: function(){
        alert("BeforeCreated")
    },
    created: function(){
        alert('Created')
    },
    beforeMount: function(){
        alert('beforeMount')
    },
    mounted: function(){
        alert('Mounted')
    },

}
</script>