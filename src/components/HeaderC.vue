<template>
    <header>
        <NavBar />
    </header>
</template>

<script>
import NavBar from './NavBar.vue';
export default {
    name: 'HeaderC',
    components: {
        NavBar
    }
}
</script>

<style lang="scss">
header {
    height: 100px;
    background-color: black;
}
</style>
