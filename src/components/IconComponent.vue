<template>
    <section class="bg-primary">
        <div class="d-flex container justify-content-evenly">
            <div v-for="(image, index) in images" :key="index" class="d-flex align-items-center">
                <img :src="image.img" alt="">
                <p>{{ image.text }}</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'IconComponent',
    data() {
        return {
            images: [
                {
                    img: '/images/buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS'
                },
                {
                    img: '/images/buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE'
                },
                {
                    img: '/images/buy-comics-shop-locator.png',
                    text: 'SUBSCRIPTION'
                },
                {
                    img: '/images/buy-comics-subscriptions.png',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    img: '/images/buy-dc-power-visa.svg',
                    text: 'DC POWER VISA'
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
section {
    height: 100px;
    padding: 20px;

    img {
        width: 50px;
        height: 65px;
    }

    p {
        color: white;
        margin-left: 10px;
    }
}
</style>