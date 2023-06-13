<template>
    <header>
        <h1>{{ title }}</h1>
        <Button text="Add Task" color="green" />
    </header>
</template>

<script lang="js">
import Button from './Button'
export default {
    // eslint-disable-next-line
    name: 'Header',
    props: {
        title: {
            type: String,
            default: 'Hello, World!'
        }
    },
    components: {
        Button
    }
};
</script>
<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>
