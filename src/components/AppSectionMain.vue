<script>
import AppCard from './AppCard.vue';
export default {
    components: { AppCard },
    props: {
        images: Array
    }

}
</script>
<template>
    <section>
        <div class=" card-container container">
            <AppCard v-for="image in images" :image="image.thumb" :serie="image.series" />
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
    padding: 2rem 0;

    .card {
        flex-basis: calc(100% / 6);
        padding: 0 10px;

    }

}
</style>