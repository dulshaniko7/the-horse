<template>
<div>
    <div class="her">
For Her
    </div>

</div>
</template>

<script>
    export default {
        name: "ForHer"
    }
</script>

<style scoped>

    .her{

        height: 90vh;
        background-position: center;
        background-image: url("../assets/girl.jpg");
        background-size: cover;
        font-size: 2.6rem;
        color:white;
        text-align: center;


        padding: 13rem;
    }
    .her:hover{
        background-image:linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)) , url("../assets/girl.jpg")  ;
        height: 90vh;
        background-position: center;


    }

</style>
