<script>
export default {
    name: "AppNavbar",

    data(){
        return{
            links:[
                'characters',
                'comics',
                'movies',
                'tv',
                'games',
                'collectibles',
                'videos',
                'fans',
                'news',
                'shop'
            ]
        }
    }
}
</script>

<template>
    <nav>

        <div id="menu">
            <div class="img-logo">
                <img src="/img/dc-logo.png" alt="">
            </div>

            <div class="menu-links">
                <ul>
                    <li v-for="currentLink in links">
                        <a href="#">
                            {{currentLink}}
                        </a>
                    </li>
                    
                </ul>
            </div>
        </div>

    </nav>
</template>

<style lang="scss">
@use '../styles/variables' as *;
@use '../styles/mixins' as *;

#menu {
    @include styleContainer;

    display: flex;
    justify-content: space-between;
    align-items: center;
}

.menu-links {

    ul {
        display: flex;
        gap: 40px;


        list-style-type: none;
        font-size: 12px;
        font-weight: 700;


        li {
            text-transform: uppercase;


            a {
                text-decoration: none;
                color: black;
                padding: 20px 0;


                &:hover {
                    color: $PrimaryColor;
                    border-bottom: 5px solid  $PrimaryColor;
                }

            }
        }
    }
}
</style>