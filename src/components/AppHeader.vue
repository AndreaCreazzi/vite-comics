<script>
import ComicCard from '../components/ComicCard.vue'
export default {
    props: { heroes: Array },
    data() {
        return {
            navbarOptions: [
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
        }
    },
    components: { ComicCard }
}
</script>

<template>
    <header>
        <nav>
            <div class="col">
                <img src="/img/dc-logo.png" alt="logo DC">
            </div>
            <div class="col">
                <ul>
                    <li v-for="navbarOption in navbarOptions" :key="navbarOption.text"><a
                            :class="{ 'active': navbarOption.current }" :url="navbarOption.url">{{ navbarOption.text }}</a>
                    </li>
                </ul>
            </div>
        </nav>
        <div class="nav-bottom">

        </div>
        <div class="card-container">
            <ComicCard :heroes="heroes" />
        </div>
        <div class="load">
            <p>LOAD MORE</p>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    height: 1200px;
    background-color: black;
}

nav {
    display: flex;
}

img {
    max-width: 70px;
}

.col {
    height: 100px;
    flex-basis: calc(100% / 2);
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: white;
}

ul {
    display: flex;
    margin-right: 80px;

    li {
        list-style-type: none;
    }

    a {
        text-decoration: none;
        font-size: 0.9rem;
        padding: 2.4rem 0.6rem;
    }
}

ul li a:hover,
.active {
    border-bottom: 3px solid #0282f9;
    color: #0282f9;
}

h2 {
    color: white;
}

.nav-bottom {
    height: 400px;
    background-image: url(/img/jumbotron.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

.card-container {
    height: 600px;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.load {
    display: flex;
    justify-content: center;
}

p {
    color: white;
    background-color: #0282f9;
    padding: 10px 70px;
}
</style>