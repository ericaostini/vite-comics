<template>
    <section class="bg-primary">
        <div class="container">
            <div class="d-flex justify-content-evenly flex-md-wrap flex-sm-wrap">
                <div v-for="(image, index) in images" :key="index"
                    class="d-flex align-items-end justify-content-between mb-md-4 mb-sm-4">
                    <img :src="image.img" alt="">
                    <p><a href="#">{{ image.text }}</a></p>
                </div>
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
    font-family: 'Open Sans', sans-serif;
    padding: 50px;

    img {
        width: 42px;
        height: 52px;
    }

    p {
        margin-left: 10px;

        a {
            color: white;
            text-decoration: none;

            &:hover {
                text-decoration: underline;
            }
        }
    }
}
</style>