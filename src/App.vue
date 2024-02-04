<script>
import AppHeader from './components/AppHeader.vue';
import AppSectionMain from './components/AppSectionMain.vue';
import AppFooterLinks from './components/AppFooterLinks.vue';
import AppFooterEndPage from './components/AppFooterEndPage.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import { navItemsHeader, iconFooter, dcComicsItem, shopItem, dcItems, sitesItems, images } from './data/index'

export default {
    components: { AppHeader, AppSectionMain, AppFooterLinks, AppFooterEndPage, AppJumbotron },
    data: () => ({
        navItemsHeader,
        iconFooter,
        dcComicsItem,
        shopItem,
        dcItems,
        sitesItems,
        images

    })

}
</script>
 
<template>
    <AppHeader :links="navItemsHeader" />
    <AppJumbotron />
    <AppSectionMain :images="images" />
    <AppFooterLinks :dc-comic-links="dcComicsItem" :shop-item="shopItem" :dc-items="dcItems" :sites-items="sitesItems" />
    <AppFooterEndPage :icons="iconFooter" />
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
