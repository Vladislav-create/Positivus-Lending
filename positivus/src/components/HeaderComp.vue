<template>
    <div class="header center">
      <!-- <h1>{{ msg }}</h1> -->
      <nav class="header__left">
        <img src="../assets/star.svg" alt="">
        <img class="header__left__logoText" src="../assets/logo.svg" alt="">
      </nav>
      <nav class="header__right">
        <a class="header__right__nav" href="#">About us</a>
        <a class="header__right__nav" href="#">Services</a>
        <a class="header__right__nav" href="#">Use Cases</a>
        <a class="header__right__nav" href="#">Pricing</a>
        <a class="header__right__nav" href="#">Blog</a>
        <button class="header__right__btn">Request a quote</button>
      </nav>
    </div>
  </template>
  
  <script>
  export default {
    name: 'HeaderComp',
    props: {
      msg: String
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style lang="scss">
  @import "../styles/variables.scss";
  @import '../styles/mixins.scss';
    a {
      text-decoration: none;
    }
    .header {
      @include center;
      display: flex;
      justify-content: space-between;
      align-items: center;
      &__left {
        @include centering;
        &__logoText {
          padding-left: 13px;
          cursor: pointer;
        }
      }
      &__right {
        display: flex;
        align-items: center;
        gap: 40px;
        &__nav {
          color: rgb(0, 0, 0);
          font-family: Space Grotesk;
          font-size: 20px;
          font-weight: 400;
          line-height: 28px;
        }
        &__btn {
          box-sizing: border-box;
          border: 1px solid rgb(25, 26, 35);
          border-radius: 14px;
          color: rgb(0, 0, 0);
          font-family: Space Grotesk;
          font-size: 20px;
          font-weight: 400;
          line-height: 28px;
          background-color: white;
          padding: 20px 35px;
          cursor: pointer;
        }
      }
    }
  
  </style>