<script>
export default {
    data: () => ({
        dcComicsItem: [
            {
                text: 'Character',
                Id: 1
            },
            {
                text: 'Comincs',
                Id: 2
            },
            {
                text: 'Movies',
                Id: 3
            },
            {
                text: 'TV',
                Id: 4
            },
            {
                text: 'Games',
                Id: 5
            },
            {
                text: 'Videos',
                Id: 6
            },
            {
                text: 'News',
                Id: 7

            },

        ],
        shopItem: [
            {
                text: ' Shop DC',
                Id: 1

            },
            {
                text: 'Shop DC Collectibles',
                Id: 2

            },
        ],
        dcItems: [
            {
                text: 'Term Of Use',
                Id: 1

            },
            {
                text: 'Privacy Policy',
                Id: 2

            },
            {
                text: 'Ad Choices',
                Id: 3

            },
            {
                text: 'Advertising',
                Id: 4

            },
            {
                text: 'Jobs',
                Id: 5

            },
            {
                text: 'Subscription',
                Id: 6

            },
            {
                text: 'Talent Workshops',
                Id: 7

            },
            {
                text: 'CPSC Certificates',
                Id: 8

            },
            {
                text: 'Ratings',
                Id: 9

            },
            {
                text: 'Shop Help',
                Id: 10

            },
            {
                text: 'Contact Us',
                Id: 11

            }
        ],
        sitesItems: [
            {
                text: 'DC',
                Id: 1

            },
            {
                text: 'MAD Magazine',
                Id: 2

            },
            {
                text: 'DC Kids',
                Id: 3

            },
            {
                text: 'DC Universe',
                Id: 4

            },
            {
                text: 'DC Power Visa',
                Id: 5

            },
        ]
    })

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
                            <li v-for="item in dcComicsItem">
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
                        <li v-for="item in dcItems">
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

