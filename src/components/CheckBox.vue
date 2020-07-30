<template>
    <input type="checkbox" :value="value" @click="CheckBox"/>
</template>

<script>
    export default {
        name: "CheckBox",
        props:['value'],
        methods: {
            CheckBox() {
                this.$emit('input',!this.value)
            }
        }
    }
</script>

<style scoped>

</style>