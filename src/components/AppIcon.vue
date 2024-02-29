<script>
export default {
    name: "AppIcon",

    data(){
        return{
            icons:[
                {
                    img:'../../public/img/buy-comics-digital-comics.png',
                    text:'digital comics'
                },
                {
                    img:'../../public/img/buy-comics-merchandise.png',
                    text:'dc merchandise'
                },
                {
                    img:'../../public/img/buy-comics-subscriptions.png',
                    text:'subscription'
                },
                {
                    img:'../../public/img/buy-comics-shop-locator.png',
                    text:'comic shop locator'
                },
                {
                    img:'../../public/img/buy-dc-power-visa.svg',
                    text:'dc power visa'
                },
            ]
        }
    }
}
</script>

<template>

    <div id="icons">

        <div class="content-icons">

            <div class="cards">
                <div class="content-card">
                    <div class="img-card">
                        <img src="../../public/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="text-card">
                        Digital comics
                    </div>
                </div>
            </div>
            <div class="cards">
                <div class="content-card">
                    <div class="img-card">
                        <img src="../../public/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="text-card">
                        Digital comics
                    </div>
                </div>
            </div>
            <div class="cards">
                <div class="content-card">
                    <div class="img-card">
                        <img src="../../public/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="text-card">
                        Digital comics
                    </div>
                </div>
            </div>
            <div class="cards">
                <div class="content-card">
                    <div class="img-card">
                        <img src="../../public/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="text-card">
                        comic shop locator
                    </div>
                </div>
            </div>
            <div class="cards">
                <div class="content-card">
                    <div class="img-card">
                        <img src="../../public/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="text-card">
                        dc merchandise
                    </div>
                </div>
            </div>

        </div>

    </div>
    
</template>

<style  lang="scss">

@use '../styles/mixins' as *;
@use '../styles/variables' as *;


#icons{
    background-color: $PrimaryColor;
}

.content-icons{
    @include styleContainer;
    padding: 60px 0;
    display: flex;
    justify-content: space-evenly;
    padding-right: 50px;

} 



.cards{
    
    

    .content-card{
        display: flex;
        align-items: center;
        gap: 20px;

        img{
            max-height: 67px;
        }

        .text-card{
            text-transform: uppercase;
            font-size: 12px;
        }
    }
}
</style>