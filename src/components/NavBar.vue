<template>
    <div class="d-flex justify-content-center flex-wrap">
        <li class="m-sm-3" :class="{ 'active': info.active }" v-for="(info, index) in informations" :key="index">
            <a href="#" class="text-dark">{{ info.text }}</a>
        </li>
    </div>
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
            ],
            activeIndex: 0
        }
    }
}
</script>

<style lang="scss" scoped>
@use '.././assets/style/partials/variables' as *;

div {
    li {
        list-style: none;
        margin-left: 20px;

        a {
            text-decoration: none;
        }
    }
}

.active {
    border-bottom: 3px outset $color-theme;
}
</style>