<template>
    <header>
        <div class="container d-flex align-items-center justify-content-between">
            <img src="/images/dc-logo.png" alt="">
            <NavBar />
        </div>
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
    height: 120px;
    background-color: white;
    border: 1px solid black;
    padding: 20px;
}

header {
    img {
        height: 75px;
        width: 75px;
    }
}
</style>
