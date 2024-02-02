<script>
export default {
    props: {
        dcComicLinks: Array,
        shopItem: Array,
        dcItems: Array,
        sitesItems: Array
    }

}

</script>
<template>
    <section id="link-footer">
        <div class="container">
            <!--LEFT SIDE-->
            <div id="left-side">
                <div id="dc-comic-links">
                    <div id="dc-comics">
                        <!--LINK DC COMICS-->
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="item in dcComicLinks">
                                <a href="">{{ item.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <!--LINK SHOP-->
                    <div id="shop-links">
                        <h3>SHOP</h3>
                        <ul>
                            <li v-for="item in shopItem">
                                <a href="">{{ item.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <!--LINK DC-->
                <div id='dc'>
                    <h3>DC</h3>
                    <ul>
                        <li v-for="item in sitesItems">
                            <a href="">{{ item.text }}</a>
                        </li>
                    </ul>
                </div>
                <!--LINK SITES-->
                <div id="sites">
                    <h3>SITES</h3>
                    <ul>
                        <li v-for="item in sitesItems">
                            <a :href="item.url">{{ item.text }}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <!--RIGHT SIDE-->
            <div id="right-side">
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
#link-footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

}

div.container {
    display: flex;
}

#left-side {
    gap: 2rem;
    margin: 0;
    flex-basis: 40%;
    display: flex;

}

#sites,
#dc,
#dc-comic-links {
    flex-basis: calc(100% / 3);
    line-height: 1.5rem;
}

#right-side {
    height: 400px;
    flex-basis: 60%;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-size: 500px;
    background-repeat: no-repeat;
    background-position: 150px -50px;
}

h3 {
    color: white;
    padding: 1rem 0;
}

ul {
    padding: 0;

    li {
        list-style: none;

    }

    a {
        color: gray;
        text-decoration: none;
    }
}
</style>

