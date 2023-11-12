<template>
    <div class="cards">
        <img :src="image" alt="serie">
        <p class="text-light text-uppercase mb-5"><small>{{ serie }}</small></p>
    </div>
</template>

<script>
export default {
    name: 'CardComponent',
    props: ["image", "serie"]
}
</script>

<style lang="scss" scoped>
.cards {
    img {
        height: 150px;
        width: 150px;
    }
}
</style>