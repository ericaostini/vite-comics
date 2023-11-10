<template>
    <main>
        <section class="section-one">
            <img src="../assets/images/jumbotron.jpg" alt="">
            <div class="container mt-5">
                <div class="row">
                    <div class="col-lg-2 col-md-4" v-for="(card, index) in myCards" :key="index">
                        <CardComponent :image="card.thumb" :serie="card.series" />
                    </div>
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

        img {
            height: 300px;
            width: 100%;
            object-fit: cover;
            object-position: top;
        }

        .mycard {
            background-color: black;
        }
    }
}
</style>../data/dc-comics