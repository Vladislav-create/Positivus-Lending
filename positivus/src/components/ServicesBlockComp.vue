<template>
    <div class="servicesBlock">
        <article 
            class="servicesBlock__cart"
            :style="{background: item.backgroundCart}"
            v-for=" item in carts" :key="item.id"
            >
            <div class="servicesBlock__cart__boxInfo">
                <div class="servicesBlock__cart__left">
                <h3 
                    :style="{background: item.backgroundText}">
                    {{ item.title }}
                </h3>
                <a class="servicesBlock__cart__left__btn" href="#">
                    <img :src="item.btn" alt="">
                    <p :style="{color: item.colorSubTitle}">Learn more</p>
                </a>
                </div>
                <div class="servicesBlock__cart__right">
                    <img :src="item.img" alt="">
                </div>
            </div>
        </article>
    </div>
</template>

<script>
    export default {
        name: 'ServicesBlockComp',
        data() {
            return {
                carts: [
                    {
                        id: 0,
                        title: 'Search engine optimisation',
                        btn: require('../assets/btnCartBlack.svg'),
                        backgroundCart: 'rgb(243, 243, 243)',
                        backgroundText: '#B9FF66',
                        colorSubTitle: 'rgb(0, 0, 0)',
                        img: require('../assets/cart1.png')
                    },
                    {
                        id: 1,
                        title: 'Pav-per-click advertising',
                        btn: require('../assets/btnCartBlack.svg'),
                        backgroundCart: '#B9FF66',
                        backgroundText: '#FFFFFF',
                        colorSubTitle: 'rgb(0, 0, 0)',
                        img: require('../assets/cart2.png')
                    },
                    {
                        id: 2,
                        title: 'Social Media Marketing',
                        btn: require('../assets/btnCartWhite.svg'),
                        backgroundCart: 'rgb(25, 26, 35)',
                        backgroundText: '#FFFFFF',
                        colorSubTitle: '#FFFFFF',
                        img: require('../assets/cart3.png')
                    },
                    {
                        id: 3,
                        title: 'Email Marceting',
                        btn: require('../assets/btnCartBlack.svg'),
                        backgroundCart: 'rgb(243, 243, 243)',
                        backgroundText: '#B9FF66',
                        colorSubTitle: 'rgb(0, 0, 0)',
                        img: require('../assets/cart4.png')
                    },
                    {
                        id: 4,
                        title: 'Content Creation',
                        btn: require('../assets/btnCartBlack.svg'),
                        backgroundCart: '#B9FF66',
                        backgroundText: '#FFFFFF',
                        colorSubTitle: 'rgb(0, 0, 0)',
                        img: require('../assets/cart5.png')
                    },
                    {
                        id: 5,
                        title: 'Analytics and Tracking',
                        btn: require('../assets/btnCartWhite.svg'),
                        backgroundCart: '#191A23',
                        backgroundText: '#B9FF66',
                        colorSubTitle: '#FFFFFF',
                        img: require('../assets/cart6.png')
                    }
                ]
            }
        }
    }
</script>

<style lang="scss">
@import "../styles/variables.scss";
@import "../styles/mixins.scss";

    .servicesBlock {
        display: flex;
        flex-wrap: wrap;
        gap: 40px;
    }
    .servicesBlock__cart {
        box-sizing: border-box;
        border: 1px solid rgb(25, 26, 35);
        border-radius: 45px;
        box-shadow: 0px 5px 0px 0px rgb(25, 26, 35);
        max-width: 600px;
        display: flex;
        &__boxInfo {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 70px;
            padding: 50px 50px;
        }
        &__left {
            text-align: left;
            & h3 {
                color: rgb(0, 0, 0);
                font-family: Space Grotesk;
                font-size: 30px;
                font-weight: 500;
                line-height: 132.6%;
                letter-spacing: 0%;
                text-align: left;
                margin: 0;
                max-width: 221px;
            }
            &__btn {
                display: flex;
                gap: 15px;
                margin-top: 93px;
                & p {
                    color: rgb(0, 0, 0);
                    font-family: Space Grotesk;
                    font-size: 20px;
                    font-weight: 400;
                    line-height: 28px;
                    letter-spacing: 0%;
                }
            }
        }
    }
</style>
