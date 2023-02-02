<script>
    export default {
        data() {
            return {
                img: 'https://unsplash.it/1000/500',
            }
        }
    }
</script>

<template>
    <div id="jumbo">
        <img :src="img" alt="jumbotron">
    </div>
</template>

<style scoped>
    #jumbo {
        position: relative;

        width: 100%;
        height: 500px;

        overflow: hidden;
    }
    #jumbo img {
        width: 100%;
        height: 100%;

        object-fit: cover;
    }
    #jumbo h2 {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);

        margin: 0;

        font-size: 4rem;
        text-transform: uppercase;
        text-shadow: 0px 0px 10px #000000;
    }
</style>