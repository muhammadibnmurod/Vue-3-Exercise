<template>
    <h1>User: {{ user.name }}</h1>
    <p>Favourite Food: {{ user.food }}</p>
    <button @click="tellParentChangeName">Change Name</button>
</template>
<script>
export default {
    props: {
        user: {
            type: Object,
            required: true
        },
    },
    methods: {
        tellParentChangeName() {
            this.$emit('change-name')
        },
    }
 
}
</script>