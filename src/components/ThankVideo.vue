<template>
    <div class="container">
        <div class="video">
            <div class="image">

            </div>
        </div>
        <div class="para">
            <h5 id="title">Kindness Isn't Cancelled</h5>
            <p>We're in a season of simplification, but we're determined to make simple as special as ever.
                Take us up on a complimentary hand written note with every online order.</p>
            <div class="explore">
                <button class="btn">Explore Gifting</button>
            </div>

        </div>

    </div>

</template>

<script>
    export default {
        name: "ThankVideo"
    }
</script>

<style scoped>
    .container {
        display: grid;
        grid-template-columns: repeat(12, 1fr);
        background-color: #f5f5f0;
        margin-top: -2rem;
    }

    .video {
        grid-column: 1/9;

    }

    .para {
        grid-column: 9/13;
        margin-top: 5rem;
        width: 20rem;

    }

    .para h5 {
        font-size: 2.5rem;
        font-weight: 100;
        margin-left: -2rem;
        margin-bottom: 1rem;
    }

    #title {

        position: relative;

    }

    #title::after {
        content: "";
        width: 15%;
        height: 1px;
        background: black;
        position: absolute;
        bottom: -5px;
        left: 0;
    }

    .para p {
        font-size: 1rem;

    }

    .explore {

    }

    .btn {
        background-color: white; /* Green */
        border: 1px solid black;
        color: black;
        padding: 1.2rem 5rem;
        text-align: center;
        cursor: pointer;
        display: inline-block;
        font-size: .8rem;
        margin: 2rem 0;
    }

    .btn:hover {
        background-color: black; /* Green */
        border: 1px solid black;
        color: white;

    }

    .image {
        height: 70vh;
        background-position: center;
        background-image: url("../assets/thanks.jpg");
        background-size: cover;
        margin: 5rem;

    }

</style>
