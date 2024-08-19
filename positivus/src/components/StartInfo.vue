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
    <div class="logoTypes center">
        <a href="https://www.amazon.com/"><img src="../assets/amazon.svg" alt=""></a>
        <a href="https://dribbble.com/"><img src="../assets/dribbble.svg" alt=""></a>
        <a href="https://www.hubspot.com/"><img src="../assets/hubspot.svg" alt=""></a>
        <a href="https://www.notion.so/"><img src="../assets/notion.svg" alt=""></a>
        <a href="https://www.netflix.com/"><img src="../assets/netflix.svg" alt=""></a>
        <a href="https://zoom.us/"><img src="../assets/zoom.svg" alt=""></a>
    </div>
    <section class="headingAndSubheading">
        <button class="headingAndSubheading__label">
            <h2>Services</h2>
        </button>
        <p>At our digital marketing agency, we offer a range of services to help businesses grow and succeed online. These services include:</p>
    </section>
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
        display: flex;
        margin-top: 70px;
        gap: 108px;
        justify-content: space-between;
        &__left {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            gap: 35px;
            &__title {
                color: rgb(0, 0, 0);
                font-family: Space Grotesk;
                font-size: 60px;
                font-weight: 500;
                line-height: 77px;
                letter-spacing: 0%;
                text-align: left
            }
            &__text {
                color: rgb(0, 0, 0);
                font-family: Space Grotesk;
                font-size: 20px;
                font-weight: 400;
                line-height: 28px;
                letter-spacing: 0%;
                text-align: left
            }
            &__btn {
                padding: 20px 35px;
                border-radius: 14px;
                background: rgb(25, 26, 35);
                color: rgb(255, 255, 255);
                font-family: Space Grotesk;
                font-size: 20px;
                font-weight: 400;
                line-height: 28px;
                letter-spacing: 0%;
                cursor: pointer;
            }
        }
    }
    .logoTypes {
        display: flex;
        gap: 96px;
        margin-top: 82px;
        margin-bottom: 151px;
    }
    .headingAndSubheading {
        display: flex;
        gap: 40px;
        margin-bottom: 85px;
        &__label {
            border: none;
            border-radius: 7px;
            background: $main-decor-color;
            padding: 7px 7px;
            & h2 {
                margin: 0;
                color: rgb(0, 0, 0);
                font-family: Space Grotesk;
                font-size: 40px;
                font-weight: 500;
                line-height: 51px;
                letter-spacing: 0%;
            }
        }
        & p {
            color: rgb(0, 0, 0);
            font-family: Space Grotesk;
            font-size: 18px;
            font-weight: 400;
            line-height: 23px;
            letter-spacing: 0%;
            max-width: 580px;
            text-align: left;
        }
    }
</style>