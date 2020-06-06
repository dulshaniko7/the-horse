<template>
    <div>
        <div class="container">


            <div class="selector">
                Trending
            </div>
            <div class="images">
                <carousel :autoplay="false" :nav="false">

                    <template slot="prev"><span class="prev pre">-----</span></template>

                    <div class="image1">
                        <div class="image-pic1">

                        </div>
                        <div class="image-wording">
                            <p>Rated 4.8 out of 5</p>
                            <p>17 Reviews</p>
                            <p>The Resin</p>
                            <p> Peach Speckle Case / White Dial / Rose Gold Indexing / Vegetable Tan Leather</p>
                            <p> 169.00</p>
                        </div>
                    </div>

                    <div class="image2">
                        <div class="image-pic2">

                        </div>
                        <div class="image-wording">
                            <p>Rated 4.8 out of 5</p>
                            <p>17 Reviews</p>
                            <p>The Resin</p>
                            <p> Peach Speckle Case / White Dial / Rose Gold Indexing / Vegetable Tan Leather</p>
                            <p> 169.00</p>
                        </div>
                    </div>
                    <div class="image3">
                        <div class="image-pic3">

                        </div>
                        <div class="image-wording">
                            <p>Rated 4.8 out of 5</p>
                            <p>17 Reviews</p>
                            <p>The Resin</p>
                            <p> Peach Speckle Case / White Dial / Rose Gold Indexing / Vegetable Tan Leather</p>
                            <p> 169.00</p>
                        </div>
                    </div>
                    <div class="image4">
                        <div class="image-pic4">

                        </div>
                        <div class="image-wording">
                            <p>Rated 4.8 out of 5</p>
                            <p>17 Reviews</p>
                            <p>The Resin</p>
                            <p> Peach Speckle Case / White Dial / Rose Gold Indexing / Vegetable Tan Leather</p>
                            <p> 169.00</p>
                        </div>
                    </div>
                    <template slot="next"><span class="next nxt">-----</span></template>
                </carousel>
            </div>
        </div>
    </div>
</template>

<script>

    import carousel from 'vue-owl-carousel'

    // import carousel from '../components/carousel'
    export default {
        name: 'Trending',
        components: {
            carousel
        }
    };
</script>

<style scoped>
    .container {

        display: grid;
        grid-template-columns: repeat(12, 1fr);
        margin: 1rem;
    }

    .selector {
        font-size: 35px;
        text-align: center;
        margin: 18rem auto;
        grid-column: 1/4;

    }


    .images {
        display: grid !important;
        grid-column: 4/13;
    }

    .image-pic1 {
        width: 300px;
        height: 405px;
        background: url("../assets/1.jpg") no-repeat;
        display: inline-block;
        background-size: cover;
    }

    .image1 {

    }

    .image2 {

    }
    .image-pic2 {
        width: 300px;
        height: 405px;
        background: url("../assets/2.jpg") no-repeat;
        display: inline-block;
        background-size: cover;
    }
    .image-pic3{
        width: 300px;
        height: 405px;
        background: url("../assets/3.jpg") no-repeat;
        display: inline-block;
        background-size: cover;
    }
    .image-pic4{
        width: 300px;
        height: 405px;
        background: url("../assets/d.jpg") no-repeat;
        display: inline-block;
        background-size: cover;
    }

    .image3 {

    }

    .image4 {

    }

    .image-pic1:hover {
        background: url("../assets/a.jpg") no-repeat;
        width: 300px;
        height: 405px;
        background-size: cover;
    }

    .image-pic2:hover {
        background: url("../assets/b.jpg") no-repeat;
        width: 300px;
        height: 405px;
        background-size: cover;
    }

    .image-pic3:hover{
        background: url("../assets/c.jpg") no-repeat;
        width: 300px;
        height: 405px;
        background-size: cover;
    }

    .image-pic4:hover {
        background: url("../assets/4.jpg") no-repeat;
        width: 300px;
        height: 405px;
        background-size: cover;
    }

    .pre {
        position: absolute;
        left: 10rem;
        top: 101rem;
        background-image: url("../assets/next.png");

    }

    .nxt {
        position: absolute;
        left: 12rem;
        top: 101rem;
        background-image: url("../assets/next.png");

    }
    .image-wording{
        text-align: center;
    }
    .image-wording  p:nth-child(1) {
        font-size: 1rem;
    }
    .image-wording  p:nth-child(2) {
        font-size: .7rem;
        color: gray;
    }
    .image-wording  p:nth-child(3) {
        margin-top: .5rem;
        font-size: 1rem;
    }
    .image-wording  p:nth-child(4) {
        margin-top: .4rem;
        font-size: .8rem;
        font-weight: bold;
    }
    .image-wording  p:nth-child(5) {
        margin-top: .4rem;
        font-size: .8rem;
        font-weight: normal;
    }

</style>
