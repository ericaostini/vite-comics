<template>
    <main>
        <section class="section-one">
            <img src="../assets/images/jumbotron.jpg" alt="">
            <div class="container mt-5 position-relative">
                <div class="my-block text-light fw-bolder">CURRENT SERIES</div>
                <div class="row justify-content-between ms-md-5 ms-lg-auto">
                    <div class="col-lg-2 col-md-4 col" v-for="(card, index) in myCards" :key="index">
                        <CardComponent :image="card.thumb" :serie="card.series" />
                    </div>
                </div>
                <div class="mx-auto d-grid ">
                    <button class="btn text-light fw-bolder mb-5">LOAD MORE</button>
                </div>
            </div>
        </section>
        <IconComponent />
    </main>
</template>

<script>
import cards from '../data/dc-comics.json'
import CardComponent from './CardComponent.vue';
import IconComponent from './IconComponent.vue';
export default {
    name: 'MainComponent',
    components: {
        IconComponent,
        CardComponent
    },
    data() {
        return {
            myCards: cards
        }
    },
}
</script>

<style lang="scss">
@use '.././assets/style/partials/variables' as *;

main {
    font-family: $main-font;

    .section-one {
        background-color: black;
        position: relative;

        .my-block {
            font-size: 18px;
            background-color: $color-theme;
            width: fit-content;
            padding: 10px 20px;
            position: absolute;
            top: -70px;
            left: -10px;
        }

        img {
            height: 300px;
            width: 100%;
            object-fit: cover;
            object-position: top;
        }

        button {
            background-color: $color-theme;
            padding: 5px 40px;
            margin: 0 auto;

            &:hover {
                border: 2px solid white;
            }
        }
    }
}
</style>../data/dc-comics