<script>

export default {
    data: () => ({
        navItems: [
            {
                text: 'Characters',
                url: '#',
                current: false,
            },
            {
                text: 'Comics',
                url: '#',
                current: true,
            },
            {
                text: 'Movies',
                url: '#',
                current: false,
            },
            {
                text: 'TV',
                url: '#',
                current: false,
            },
            {
                text: 'Games',
                url: '#',
                current: false,
            },
            {
                text: 'Collectibles',
                url: '#',
                current: false,
            },
            {
                text: 'Videos',
                url: '#',
                current: false,
            },
            {
                text: 'Fans',
                url: '#',
                current: false,
            },
            {
                text: 'News',
                url: '#',
                current: false,
            },
            {
                text: 'Shop',
                url: '#',
                current: false,
            },
        ]
    }),






}
</script>
<template>
    <header class="container">
        <picture><img role="button" src="../assets/img/dc-logo.png" alt=""></picture>
        <nav>
            <ul>
                <li :class="{ 'active': item.current === true }" @click="changeCurrentValue" role="button"
                    v-for="item in  navItems">
                    <a :href="item.url"></a>{{ item.text }}
                </li>
            </ul>
        </nav>
    </header>
</template>
<style>
header {
    display: flex;
    align-items: center;
    font-weight: bold;
    padding: 1.5rem 0;
    gap: 12rem;
}

ul {
    display: flex;
    list-style: none;
    gap: 1.5rem;
    font-size: 0.75rem;
    text-transform: uppercase;
}

li {
    padding: 3rem 0;
    cursor: pointer;

}

li.active {
    color: #0282F9;
    border-bottom: 5px solid #0282F9;
}
</style>