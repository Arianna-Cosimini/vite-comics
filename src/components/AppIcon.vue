<script>
export default {
    name: "AppIcon",

    data() {
        return {
            icons: [
                {
                    img: '../../public/img/buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    img: '../../public/img/buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    img: '../../public/img/buy-comics-subscriptions.png',
                    text: 'subscription'
                },
                {
                    img: '../../public/img/buy-comics-shop-locator.png',
                    text: 'comic shop locator'
                },
                {
                    img: '../../public/img/buy-dc-power-visa.svg',
                    text: 'dc power visa'
                },
            ]
        }
    }
}
</script>

<template>

    <div id="icons">

        <div class="content-icons">

            <div v-for="(currentIcon, index) in icons" class="cards">
                <div class="content-card">
                    <div class="img-card">
                        <img :src='currentIcon.img' :style="{ height: index < 4 ? '67px' : '45px' }">
                    </div>
                    <div class="text-card">
                        {{ currentIcon.text }}
                    </div>
                </div>
            </div>


        </div>

    </div>
</template>

<style  lang="scss">
@use '../styles/mixins' as *;
@use '../styles/variables' as *;


#icons {
    background-color: $PrimaryColor;
    position: relative;
    z-index: 1;
}

.content-icons {
    @include styleContainer;
    padding: 60px 0;
    display: flex;
    justify-content: space-evenly;
    padding-right: 50px;

}



.cards {

    display: flex;
    align-items: center;


    .content-card {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 20px;

        .img-card {
            max-height: 67px;
        }

        .text-card {
            text-transform: uppercase;
            font-size: 12px;
        }
    }
}
</style>