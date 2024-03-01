<script>
export default {
    name: 'CardItems',

   
    props: {
        // dobbiamo dare un nome a queste proprietà
        // per ognuna di esse dobbiamo indicare nome e TIPO DI DATO
        // String, Number, Boolean, Array, Object
        // il tipo di dato deve iniziare con la lettera maiuscola
        cardName: String,
        cardImage: String
    },

    data() {
    },
}
</script>

<template>

    <div class="cards">
        <img :src="cardImage" :alt="cardName">
        <h4>{{ cardName }}</h4>
    </div>

</template>

<style lang="scss">

.cards{
    display: flex;
    flex-direction: column;
    
    width: calc(100% / 6 - 20px);
    padding: 20px 0;

    img{
        max-height: 185px;
        object-fit: cover;
        width: 100%;
    }
}

</style>