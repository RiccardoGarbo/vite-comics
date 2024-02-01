<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
export default {
    components: { AppHeader, AppMain }

}
</script>

<template>
    <AppHeader />
    <AppMain />
</template>

<style>
/*Generics*/

* {
    padding: 0 auto;
    margin: 0 auto;
    box-sizing: border-box;
}

body {
    min-height: 100vh;
    font-family: "Open Sans", sans-serif;
}

/*Utils*/
.container {
    width: 1080px;
    margin: 0 auto;
}

img {
    max-width: 100%;
    display: block;

}
</style>
