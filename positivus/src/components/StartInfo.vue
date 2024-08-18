<template>
    <div class="startInfo center">
        <div class="startInfo__left">
            <h1 class="startInfo__left__title">Navigating the digital landscape for success</h1>
            <p class="startInfo__left__text">Our digital marketing agency helps businesses grow and succeed online through a range of services including SEO, PPC, social media marketing, and content creation.</p>
            <button class="startInfo__left__btn">Book a consultation</button>
        </div>
        <div class="startInfo__right">
            <img src="../assets/Illustration.svg" alt="">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'StartInfo',

    }
</script>

<style lang="scss">
    @import "../styles/variables.scss";
    @import '../styles/mixins.scss';
    .startInfo {
        @include center;
        display: flex;
        margin-top: 70px;
        &__left {
            display: flex;
            flex-direction: column;
        }
    }

</style>