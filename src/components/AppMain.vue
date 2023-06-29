<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <main>
        <div class="row">
            <div class="col">
                <h3>DC COMICS</h3>
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movie</a></li>
                    <li><a href="#">Tv</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Video</a></li>
                    <li><a href="#">News</a></li>
                </ul>
                <h3>SHOP</h3>
                <ul>
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collactibles</a></li>
                </ul>
            </div>
            <div class="col">
                <h3>DC</h3>
                <ul>
                    <li><a href="#">Terms of Use</a></li>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Ad Chorse</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscriptions</a></li>
                    <li><a href="#">Talent Worksop</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#"> Shop Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>
            <div class="col">
                <h3>SITES</h3>
                <ul>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC Universe</a></li>
                    <li><a href="#">DC Power Visa</a></li>
                </ul>
            </div>
        </div>
    </main>
</template>

<style scoped>
main {
    background-image: url(/img/dc-logo-bg.png), url(img/footer-bg.jpg);
    background-position: right 30% top 30%, center;
    background-repeat: no-repeat;
    background-size: 450px, cover;
}

.row {
    display: flex;
    height: 350px;
}

.col:first-child {
    margin-left: 250px;
}

.col {
    padding: 0 20px;
}

h3 {
    color: white;
    margin-top: 20px;
    margin-bottom: 10px;
}

ul li {
    list-style-type: none;
}

ul li a {
    text-decoration: none;
    font-size: 0.8rem;
    color: #737578;
}
</style>