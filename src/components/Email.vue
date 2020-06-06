<template>

    <div class="bar">
        <label class="bar-p">Want news from the Stable plus 10% off your first order?</label>
        <input type="text" placeholder="Kindly enter your email address                      >">
    </div>

</template>

<script>
    export default {
        name: "Email"
    }
</script>

<style scoped>


    .bar {
        margin: .5rem 0;
        background-color: #f5f5f0;
        padding: 2.2rem;
        display: grid;
        grid-template-columns: repeat(12, 1fr);
    }

    .bar label {
        width: 200px;
        grid-column: 4/6;
        font-size: .9rem;
    }

    .bar input[type=text] {
        width: 300px;
        grid-column: 6/9;
        border: none;
        border-bottom: 1px solid gray;
        background-color: #f5f5f0;
        font-size: .9rem;

    }
     input:focus {
border: none;
        background-color: #f5f5f0;
         outline: none !important
    }
</style>
