<template>
    <footer>
        <p>Copyright &copy; 2023</p>
        <router-link to="/about">About</router-link>
    </footer>
</template>

<script lang="js">
export default {
    // eslint-disable-next-line
    name: 'Footer'
}
</script>

<style scoped>
a {
    color: #333;
}

footer {
    margin-top: 30px;
    text-align: center;
}
</style>
