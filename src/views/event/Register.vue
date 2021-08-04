<template>
    <p>Register for the event here</p>
    <button class="button" @click="onRegister">Let's register!</button>
</template>

<script>
export default {
    props: ['event'],
    methods: {
        onRegister() {
            this.$router.push({
                name: 'EventDetails'
            })
        }
    }
}
</script>

<style scoped>
.button {
    cursor: pointer;
    padding: .5rem 1rem;
}
</style>
