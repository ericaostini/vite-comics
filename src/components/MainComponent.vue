<template>
    <main>
        <section class="section-one">
            <img src="../assets/images/jumbotron.jpg" alt="">
        </section>
        <IconComponent />
    </main>
</template>

<script>
import IconComponent from './IconComponent.vue';
export default {
    name: 'MainComponent',
    components: {
        IconComponent,
    }
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

        p {
            color: white;
            margin: 0;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }
    }
}
</style>