<script>
export default {
    name: "AppContent",
}
</script>

<template>
    <div id="content">
        <div class="text-content">
            <span>Content goes here</span>
        </div>
    </div>
</template>

<style  lang="scss">

@use '../styles/mixins' as *;
@use '../styles/variables' as *;

#content {
    background-color: #000;

}

.text-content{
    @include styleContainer;
    padding: 60px 0;

    span:before{
        content: '-->';
        padding-right: 5px;

    }


    &::after{
        content: '<--';
        padding-left: 5px;

    }
} 
</style>