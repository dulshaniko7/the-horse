<template>
    <div>
        <div class="image">
            <div class="heading">
                <h1>THE MONOGRAM SHOP</h1>
                <p>OUR PERSONALISATION SERVICE NOW OPEN</p>
                <img class="arrow" src="../assets/arrow.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "MonogramShop"
    }
</script>

<style scoped>
    .image {
        height: 110vh;
        margin-top: -3rem;
        background-image: url("../assets/tools.jpg");
        background-size: cover;
        display: grid;
        grid-template-columns: repeat(12, 1fr);
        grid-template-rows: repeat(2, 1fr);
        margin-bottom: 2rem;
    }

    .heading {
        grid-column: 10/13;
        letter-spacing: 3px;
        grid-row: 2/3;
        color: white;

    }

    .heading h1 {

        font-size: 3rem;
        margin-bottom: 2.5rem;
    }

    .heading p {
        font-size: .8rem;
        color: white;
        font-weight: normal;
        width: 250px;
    }

    .arrow {
        width: 81px;

        margin-top: 1rem;
    }

</style>
