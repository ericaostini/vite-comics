<template>
    <section class="bg-primary">
        <div>
            <img src="" alt="">
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
    height: 120px;
}
</style>