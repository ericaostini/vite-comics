<template>
    <footer>
        <section class="footer-top">
            <div class="container d-flex justify-content-between">
                <ul v-for="(info, index) in footerInfos" :key="index">
                    <li>{{ info.title }}</li>
                    <li v-for="(i, index) in info.inform"><small>{{ i }}</small></li>
                </ul>
                <img src="/images/dc-logo-bg.png" alt="">
            </div>
        </section>
        <section class="footer-bottom">
            <div class="container d-flex justify-content-between align-items-center">
                <button class="btn text-light">SIGN-UP NOW</button>
                <div class="d-flex align-items-center">
                    <div class="mx-3 text-info">FOLLOW US</div>
                    <img v-for="(icon, index) in icons" :src="icon" alt="">
                </div>
            </div>
        </section>
    </footer>
</template>

<script>
export default {
    name: 'FooterComponents',
    data() {
        return {
            footerInfos: [
                {
                    title: 'DC COMICS',
                    inform: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
                },
                {
                    title: 'DC',
                    inform: ['Terms Of Use', 'Privacy policy', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
                },
                {
                    title: 'SITES',
                    inform: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
                },
                {
                    title: 'SHOP',
                    inform: ['Shop DC', 'Shop DC Collectibles']
                },

            ],
            icons: ['/images/footer-facebook.png', '/images/footer-periscope.png', '/images/footer-pinterest.png', '/images/footer-twitter.png', '/images/footer-youtube.png']
        }
    },
}
</script>

<style lang="scss" scoped>
footer {
    .footer-top {
        background-image: url("../images/footer-bg.jpg");
        height: 370px;
        overflow: hidden;

        li {
            color: white;
            list-style: none;
        }

        img {
            height: 450px;
            position: relative;
            top: -60px;
        }
    }

    .footer-bottom {
        background-color: rgb(51, 50, 50);
        height: calc(100vh - 670px);
        padding: 30px;

        button {
            border: 1px solid blue;
            padding: 10px;

        }

        img {
            width: 30px;
            height: 30px;
            margin-right: 10px;
        }
    }
}
</style>