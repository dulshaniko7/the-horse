<template>
    <div class="container">
        <div class="her">
            <ForHer></ForHer>
        </div>
        <div class="him">
            <ForHim></ForHim>
        </div>
    </div>
</template>

<script>
    import ForHer from "./ForHer";
    import ForHim from "./ForHim";

    export default {
        name: "GirlOrBoy",
        components: {ForHim, ForHer}
    }
</script>

<style scoped>
    .container {
        display: grid;
        grid-template-columns: repeat(12, 1fr);
        margin: 1.5rem;
        grid-gap: 1.5rem;
    }

    .her {
        grid-column: 1/7;


    }

    .him {
        grid-column: 7/13;


    }


</style>
