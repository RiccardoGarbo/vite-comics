<script>
export default {
    props: {
        icons: Array
    }

}
</script>
<template>
    <footer>
        <div id="footer-end" class="container">
            <input type="button" value="SIGN-UP NOW!">
            <div id="link-footer-end">
                <ul>
                    <li id="followUS">FOLLOW US</li>
                    <li v-for="icon in icons "> <a :href="icon.url"><img :src="`/img/footer-${icon.image}`"
                                :alt="icon.name"> </a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
input {
    padding: 1rem;
    border: 2px solid #0282F9;
    background-color: #303030;
    color: white;
    margin: 2rem 0;
    cursor: pointer;
}

footer {
    background-color: #303030;

}

#footer-end {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 15rem;


}


ul {
    display: flex;
    align-items: center;
    gap: 1rem;


    li {
        list-style: none;
    }


    a {
        color: white;
        text-decoration: none;

    }
}

#followUS {
    font-weight: 700;
    color: #0282F9
}
</style>
