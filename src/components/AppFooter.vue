<script>
export default {
    name: "AppFooter",

    data() {
        return {
            footerLinks: [
                {
                    title: 'dc comics',
                    list: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                    ]
                },
                {
                    title: 'dc',
                    list: [
                        'Terms Of Use',
                        'Privacy Policy (New)',
                        'Ad Choice',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us',


                    ]
                },
                {
                    title: 'sites',
                    list: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa',
                    ]
                },
                {
                    title: 'shop',
                    list: [
                        'Shop DC',
                        'Shop DC Collectibles',
                    ]
                },
            ],
        }
    }
}
</script>

<template>
    <footer>
        <div class="content-footer">

            <div class="footer-menu">
                <div v-for="linkList in footerLinks" class="footer-links">
                    <h3>{{ linkList.title }}</h3>
                    <ul>
                        <li v-for="currentLink in linkList.list">
                            <a href="#">
                                {{ currentLink }}
                            </a>
                        </li>

                    </ul>
                </div>


            </div>

            <div class="footer-img">
                <img src="../../public/img/dc-logo-bg.png" alt="">
            </div>
        </div>

        <div class="footer-icon">
            <div class="content-footer-icon">

                <div class="btn-footer">
                    <button type="button">SIGN-UP NOW!</button>
                </div>

                <div class="icon">
                    <div class="text-icon">
                        <span>follow us</span>
                    </div>

                    <div class="social-icons">
                        <img src="../../public/img/footer-facebook.png" alt="">
                        <img src="../../public/img/footer-twitter.png" alt="">
                        <img src="../../public/img/footer-youtube.png" alt="">
                        <img src="../../public/img/footer-pinterest.png" alt="">
                        <img src="../../public/img/footer-periscope.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style  lang="scss">
@use '../styles/mixins' as *;
@use '../styles/variables' as *;


footer {
    background-image: url('../../public/img/footer-bg.jpg');
    background-size: cover;
    background-position: bottom;

}

.content-footer {
    @include styleContainer;
    display: flex;
    justify-content: space-between;


}

.footer-menu {
    display: flex;
    gap: 50px;
    flex-wrap: wrap;
    padding-top: 50px;
    padding-bottom: 140px;

    .footer-links {
        margin-bottom: -140px;

        h3 {
            text-transform: uppercase;
            font-size: 20px;

            margin: 0;
        }

        ul {
            list-style-type: none;
            padding: 0;
        }

        a {
            text-decoration: none;
            color: #808178;
        }
    }

}

.footer-img {
    margin: -90px 0;
    position: relative;
    z-index: 0;

    img {
        z-index: 0;
    }
}

.footer-icon {


    background-color: #303030;
    padding: 37px 0;
    position: relative;
    z-index: 1;

    .content-footer-icon {
        @include styleContainer;

        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    button {
        padding: 18px 12px;
        font-size: 16px;

        background-color: transparent;
        border: 2px solid $PrimaryColor;
    }

    .text-icon{
        span{
            text-transform: uppercase;
            font-size: 20px;
            font-weight: 700;
            color: $PrimaryColor;
        }
    }

    .icon{
        display: flex;
        gap: 35px;


        .social-icons{
            display: flex;
            gap: 20px;
        }
    }
}


</style>