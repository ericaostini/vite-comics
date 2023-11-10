<template>
    <div class="col-4">
        <img :src="image" alt="serie">
        <p><strong>{{ serie }}</strong></p>
    </div>
</template>

<script>
export default {
    name: 'CardComponent',
    props: ["image", "serie"]
}
</script>

<style lang="scss" scoped></style>