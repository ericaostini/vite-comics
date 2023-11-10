<template>
    <footer>
        <section class="footer-top">
            <div class="container d-flex justify-content-between">
                <div>
                    <div class="d-flex">
                        <ul v-for="(info, index) in footerInfos" :key="index">
                            <li class="fw-bolder">{{ info.title }}</li>
                            <li v-for="(i, index) in info.inform" class="small-title"><small>{{ i }}</small>
                            </li>
                        </ul>
                    </div>
                    <ul class="info-relative">
                        <li class="fw-bolder">SHOP</li>
                        <li><small>Shop DC</small></li>
                        <li><small>Shop DC</small></li>
                    </ul>
                </div>
                <img class="position-relative" src="/images/dc-logo-bg.png" alt="">
            </div>
        </section>
        <section class="footer-bottom">
            <div class="container d-flex justify-content-between align-items-center">
                <button class="btn text-light fw-bolder">SIGN-UP NOW</button>
                <div class="d-flex align-items-center">
                    <div class="mx-3 text-light fw-bolder followUS">FOLLOW US</div>
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
                }

            ],
            icons: ['/images/footer-facebook.png', '/images/footer-periscope.png', '/images/footer-pinterest.png', '/images/footer-twitter.png', '/images/footer-youtube.png']
        }
    },
}
</script>

<style lang="scss" scoped>
@use '.././assets/style/partials/variables' as *;

footer {
    font-family: $main-font;

    .footer-top {
        background-image: url("../images/footer-bg.jpg");
        overflow: hidden;
        height: 450px;

        .info-relative {
            position: relative;
            bottom: 126px;

            small {
                color: $color-smalltext;
            }
        }

        ul {
            padding-top: 40px;
            padding-right: 40px;

            li {
                color: white;
                list-style: none;
            }

            .small-title {
                color: $color-smalltext;

                &:hover {
                    color: white;
                }
            }
        }

        img {
            position: relative;
            top: -50px;
        }
    }

    .footer-bottom {
        background-color: $color-footer;
        height: calc(100% - 670px);
        padding: 30px;

        button {
            border: 1px solid $color-theme;
            padding: 10px;

            &:hover {
                background-color: $color-theme;
            }

        }

        img {
            width: 30px;
            height: 30px;
            margin-right: 10px;
        }
    }
}
</style>