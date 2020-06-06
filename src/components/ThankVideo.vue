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
                hi
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
    .explore{
        border: 2px solid red;
    }

    .image {
        height: 70vh;
        background-position: center;
        background-image: url("../assets/thanks.jpg");
        background-size: cover;
        margin: 5rem;

    }

</style>
