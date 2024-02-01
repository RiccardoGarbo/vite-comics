<script>
import AppHeader from './components/AppHeader.vue';
import AppSectionMain from './components/AppSectionMain.vue';
import AppFooterLinks from './components/AppFooterLinks.vue';

export default {
    components: { AppHeader, AppSectionMain, AppFooterLinks }

}
</script>

<template>
    <AppHeader />
    <AppSectionMain />
    <AppFooterLinks />
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
