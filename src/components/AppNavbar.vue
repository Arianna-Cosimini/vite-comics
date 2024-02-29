<script>
export default {
    name: "AppNavbar",
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
                    <li>
                        <a href="#">
                            characters
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            comics
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            movies
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            tv
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            games
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            collectibles
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            videos
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            fans
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            news
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            shop
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