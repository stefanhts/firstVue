<template>
    <header>
        <h1>{{title}}</h1>
        <Button text="Add Task" color = "Green"/>
    </header>
</template>

<script>
import Button from './Button'

export default{
    name:"Header",
    components: {
        Button,
    },
    props: {
        title: {
            type: String,
            default: 'Hello World'
        }
    }
}
</script>

<style scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom:20px;
}
</style>