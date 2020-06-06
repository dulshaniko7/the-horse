<template>
    <div id="app">
        <TopNav></TopNav>
        <MainPicture></MainPicture>
        <Email></Email>

        <GirlOrBoy></GirlOrBoy>
        <Trending></Trending>

        <carousel ></carousel>
        <MonogramShop></MonogramShop>
        <ThankVideo></ThankVideo>
        <Slider></Slider>
        <Explore></Explore>
        <ShopNow></ShopNow>
        <Footer></Footer>
    </div>
</template>

<script>
    import TopNav from "./components/TopNav"

    import Email from "./components/Email";

    import Trending from "./components/Trending";
    import MonogramShop from "./components/MonogramShop";
    import ThankVideo from "./components/ThankVideo";
    import Slider from "./components/Slider";
    import Explore from "./components/Explore";
    import ShopNow from "./components/ShopNow";
    import Footer from "./components/Footer";
    import MainPicture from "./components/MainPicture";
    import GirlOrBoy from "./components/GirlOrBoy";


    export default {

        name: 'App',

                components: {

                    GirlOrBoy,
                    MainPicture,
                    Footer,
                    ShopNow,
                    Explore,
                    Slider,
                    ThankVideo,
                    MonogramShop,
                    Trending,
                    Email,
                    TopNav,

                }

        }

</script>

<style>
    #app {

    }

    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }

</style>
