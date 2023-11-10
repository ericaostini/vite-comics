<template>
    <img :src="image" alt="serie">
    <p class="text-light text-uppercase mb-5 "><small>{{ serie }}</small></p>
</template>

<script>
export default {
    name: 'CardComponent',
    props: ["image", "serie"]
}
</script>

<style lang="scss" scoped></style>