<template>
    <div>
        <div class="him">
            For Him
        </div>
    </div>
</template>

<script>
    export default {
        name: "ForHim"
    }
</script>

<style scoped>
    .him {
        height: 90vh;
        background-position: center;
        background-image: url("../assets/boy.jpg");
        background-size: cover;
        font-size: 2.6rem;
        color: white;
        text-align: center;
        padding: 13rem;
    }
    .him:hover{
        background-image:linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)) , url("../assets/boy.jpg")  ;
        height: 90vh;
        background-position: center;


    }

</style>
