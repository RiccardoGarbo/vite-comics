<script>
export default {
    props: {
        images: Array
    }

}
</script>
<template>
    <section>
        <div class=" card-container container">
            <div v-for="image in images" class="card">
                <div>
                    <img :src="image.thumb" alt="">
                    <h5>{{ image.series }}</h5>
                </div>

            </div>
        </div>
    </section>
</template>
<style scoped>
section {
    background-color: #1C1C1C;
}

.card-container {
    display: flex;
    flex-wrap: wrap;


    .card {
        flex-basis: calc(100% / 6);
        padding: 20px;

    }

    img {
        display: block;
        height: 200px
    }

    h5 {
        color: white
    }

}
</style>