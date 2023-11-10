<template>
    <main>
        <section class="section-one">
            <img src="../assets/images/jumbotron.jpg" alt="">
            <div class="container mt-5 position-relative ">
                <div class="my-block text-light fw-bolder">CURRENT SERIES</div>
                <div class="row">
                    <div class="col-lg-2 col-md-4" v-for="(card, index) in myCards" :key="index">
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
main {
    font-family: 'Open Sans', sans-serif;

    .section-one {
        background-color: black;
        position: relative;

        .my-block {
            background-color: #0C6DFD;
            width: fit-content;
            padding: 5px 15px;
            position: absolute;
            top: -60px;
            left: -10px;
        }

        img {
            height: 300px;
            width: 100%;
            object-fit: cover;
            object-position: top;
        }

        button {
            background-color: #0C6DFD;
            padding: 5px 40px;
            margin: 0 auto;

            &:hover {
                border: 2px solid white;
            }
        }
    }
}
</style>../data/dc-comics