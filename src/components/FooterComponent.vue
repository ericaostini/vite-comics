<template>
    <footer>
        <section class="footer-top">
            <div class="container d-flex">
                <ul v-for="(info, index) in footerInfos" :key="index">
                    <li>{{ info.title }}</li>
                    <li v-for="(i, index) in info.inform"><small>{{ i }}</small></li>
                </ul>
                <img src="" alt="">
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

            ]
        }
    },
}
</script>

<style lang="scss" scoped>
footer {
    .footer-top {
        background-image: url("../images/footer-bg.jpg");
        height: 320px;

        li {
            color: white;
            list-style: none;
        }
    }
}
</style>