<template>
    <main>
        <section class="section-one">
            <p class="container">--Content goes here--</p>
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
    .section-one {
        height: 120px;
        background-color: black;
        position: relative;

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