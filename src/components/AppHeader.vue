<script>
export default {
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
    }
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
    </header>
</template>

<style lang="scss" scoped>
header {
    height: 1100px;
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
    background-image: url(../../public/img/jumbotron.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}
</style>