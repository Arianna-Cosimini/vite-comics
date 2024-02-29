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
                    <li>characters</li>
                    <li>comics</li>
                    <li>movies</li>
                    <li>tv</li>
                    <li>games</li>
                    <li>collectibles</li>
                    <li>videos</li>
                    <li>fans</li>
                    <li>news</li>
                    <li>shop</li>
                </ul>
            </div>
        </div>

    </nav>
</template>

<style lang="scss">

#menu{
    max-width: 1200px;
    margin: 0 auto;

    display: flex;
    justify-content: space-between;
}



</style>