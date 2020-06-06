<template>
    <div>
        <div class="image">
            <div class="saying">
                <h1>THE NEW RESIN RANGE</h1>
                <p>Explore the Collections</p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "MainPicture"
    }
</script>

<style scoped>
    * {
        margin: 0;
        padding: 0;
    }

    .image {
        height: 90vh;
        background-position: center;
        background-image: url("../assets/image2.jpg");
        background-size: cover;
        display: grid;
        grid-template-columns: repeat(12, 1fr);

    }

    .saying {
        grid-column: 1/4;
        font-size: 1.2rem;
        text-align: center;
        margin: auto;

    }

    .saying h1 {
        letter-spacing: 6px;
        color: steelblue;

    }

    .saying p {

    }

</style>
