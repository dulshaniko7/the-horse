<template>
    <div>

        <div class="navi">
            <img src="../assets/icons8-lines.png" alt="" class="nav-line" v-on:click="navList">
            <div class="small-nav" v-show="small">
                <ul>
                    <li>Search</li>
                    <li>WOMEN'S</li>
                    <li>MEN'S</li>
                    <li>GIFTING</li>
                    <li>THE MONOGRAM SHOP</li>
                    <li>SALE</li>
                </ul>
            </div>

            <div class="list">
                <ul class="list-ui">
                    <li class="list-li">WOMEN'S</li>
                    <li class="list-li">MEN'S</li>
                    <li class="list-li">GIFTING</li>
                    <li class="list-li">THE MONOGRAM SHOP</li>
                    <li class="list-li">SALE</li>
                </ul>
            </div>
            <div class="title">
                <h4 class="title1">THE</h4>
                <h4 class="title2">HORSE</h4>
            </div>
            <div class="shoppingCart">
                <div>
                    <p class="nav-p" v-on:click="showCurrency">{{c}} {{listIcon}}</p>
                </div>
                <div class="currency-list" v-show="show">
                    <p v-for="(c,index) in currencyList" v-bind:key="index" v-on:click="hideCurrency(c.currency)">
                        {{c.currency}} / $</p>
                </div>
                <div class="nav-icons">
                    <img src="../assets/icons8-user-24.png" class="nav-icon">
                    <img src="../assets/icons8-search-26.png" alt="" class="nav-icon">
                    <img src="../assets/icons8-shopping-cart.png" alt="" class="nav-icon">
                </div>
            </div>
        </div>


    </div>

</template>

<script>


    export default {

        name: "TopNav",

        data() {
            return {
                show: false,
                showNav: false,
                listIcon: 'v',
                small: false,
                c: 'AUD',
                currencyList: [
                    {currency: 'AUD  '},

                    {currency: 'CAD  '},

                    {currency: 'EUR  '},

                    {currency: 'GBP  '},

                    {currency: 'JPY  '},

                    {currency: 'NZD  '},

                    {currency: 'USD  '}
                ]
            }
        },
        methods: {
            showCurrency() {
                this.show = !this.show
                this.listIcon = "^"

            },
            hideCurrency(c) {
                this.listIcon = "v"
                this.show = !this.show
                this.c = c

            },

            navList() {
                this.small = !this.small
            }


        }

    }
</script>

<style scoped>
    .navi {
        display: grid;
        grid-template-columns: repeat(12, 1fr);
        background: white;
        border-bottom: 1px solid gainsboro;
    }

    .list {
        vertical-align: middle;
        line-height: 5rem;
        text-align: center;
        font-size: .9rem;
        color: dimgray;
        grid-column: 1/6;
        z-index: 2;
    }

    .list-ui {
        float: left;
    }

    .list-li {
        float: left;
        list-style: none;
        margin: 0 .5rem;
    }

    .list-li:nth-child(5) {
        color: red;
    }

    .title {
        letter-spacing: .4rem;
        font-size: 1.4rem;
        line-height: 0.3rem;
        grid-column: 6/8;
        margin: auto;
    }

    .title1 {
        float: left;
        color: dimgray;
    }

    .title2 {
        float: left;
    }

    .shoppingCart {

        grid-column: 8/13;
        margin-left: 18rem;

    }

    .nav-icons {
        margin-left: 1rem;
        margin-top: 1rem;
    }

    .nav-icon {
        margin-left: 1.5rem;
    }

    .nav-p {
        float: left;
        line-height: 4rem;
        font-size: 1rem;
        letter-spacing: 2px;
    }

    .currency-list {
        position: absolute;
        margin-top: 3rem;
        background-color: white;
        padding-bottom: 1rem;

        font-size: .9rem;
    }

    .currency-list p {
        padding-left: .7rem;
        padding-right: .7rem;
        padding-top: .7rem;
    }

    .small-nav {

    }

    .small-nav ul {
        display: block;
        list-style: none;

    }

    .small-nav li {
        width: 50rem;
    }

    * {
        margin: 0;
        padding: 0;
    }


    @media screen and (max-width: 620px) {
        .navi {
            display: grid;
            grid-template-columns: repeat(12, 1fr);
            background: white;
            border-bottom: 1px solid gainsboro;
        }


        .title {
            letter-spacing: .1rem;
            font-size: .6rem;
            line-height: 0.3rem;
            grid-column: 4/8;
            margin: auto;
        }

        .list {
            display: none;
        }

        .shoppingCart {
            margin-left: 4rem;
        }

        .nav-icon {
            margin-left: .5rem;
        }

        .nav-icon:nth-child(1) {
            display: none;
        }

    }

    @media screen and (max-width: 1200px) {

        .navi {
            display: grid;
            grid-template-columns: repeat(12, 1fr);
            background: white;
            border-bottom: 1px solid gainsboro;
        }

        .title {
            letter-spacing: .1rem;
            font-size: 1.1rem;
            line-height: 0.3rem;
            grid-column: 3/8;
            margin: auto;
        }

        .list-li {
            font-size: .7rem;
            margin: 0 .1rem;

        }

        .nav-icon {
            margin-left: .5rem;
        }

        .list {
            display: none;
        }

        .nav-icon:nth-child(1) {
            display: none;
        }

        .shoppingCart {
            margin-left: 2rem;
        }

        .nav-line {

        }

    }

    @media screen and (min-width: 1200px) {
        .nav-line {
            display: none;
        }

        .small {
            display: none;
        }

        .shoppingCart {
            margin-left: 18rem;
        }

    }

</style>
