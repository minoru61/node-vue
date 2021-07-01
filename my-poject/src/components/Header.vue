<template>
    <header>
        <h2>{{ title }}</h2>
        <Button @click="onClick()" text="Edit Profile" color="steelblue"/>
    </header>
</template>

<script>
    import Button from './Button'
    export default {
        name:'Header',
        props:{
            title: String,
        },
        components: {
            Button
        },
        methods: {
            onClick() {
                console.log('Click')
            },
        },
    }
</script>

<style scoped>
header {
    display : flex;
    justify-content : space-between;
    align-items : center;
    margin-bottom : 20px;
}
</style>