<script>
export default {
    props: {
        image: String,
        serie: String
    }

}
</script>
<template>
    <div class="card">
        <img :src="image" alt="">
        <h5>{{ serie }}</h5>
    </div>
</template>
<style scoped>
img {
    display: block;
    width: 200px;
    height: 200px;
    margin: 0;
    scale: 1
}

h5 {
    color: white;
    padding: 1rem 0;
}
</style>