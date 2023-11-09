<template>
    <header>
        <div class="container d-flex align-items-center justify-content-between flex-nowrap">
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
    background-color: white;
    padding: 15px;
    font-family: 'Passion One', sans-serif;
}

header {

    img {
        height: 75px;
        width: 75px;
    }
}
</style>
