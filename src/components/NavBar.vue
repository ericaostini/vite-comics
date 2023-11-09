<template>
    <nav class="nav container justify-content-end">
        <li class="nav-link text-dark" :class="{ 'active': info.active }" v-for="(info, index) in informations"
            :key="index">{{
                info.text }}</li>
    </nav>
</template>

<script>
export default {
    name: 'NavBar',
    data() {
        return {
            informations: [
                {
                    text: 'CHARACTERS',
                    active: false,
                },
                {
                    text: 'COMICS',
                    active: true,
                },
                {
                    text: 'MOVIES',
                    active: false,
                },
                {
                    text: 'TV',
                    active: false,
                },
                {
                    text: 'GAMES',
                    active: false,
                },
                {
                    text: 'COLLECTIBLES',
                    active: false,
                },
                {
                    text: 'VIDEOS',
                    active: false,
                },
                {
                    text: 'FANS',
                    active: false,
                },
                {
                    text: 'NEWS',
                    active: false,
                },
                {
                    text: 'SHOP',
                    active: false,
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
nav {
    li {
        color: black;
    }
}

.active {
    border-bottom: 2px solid #0C6DFD;
}
</style>