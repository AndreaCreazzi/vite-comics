<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <footer>
        <div class="row">
            <div class="col">
                <h4>SIGN-UP NOW!</h4>
            </div>
            <div class="col">
                <h3>FOLLOW US</h3>
                <img src="/img/footer-facebook.png" alt="">
                <img src="/img/footer-periscope.png" alt="">
                <img src="/img/footer-pinterest.png" alt="">
                <img src="/img/footer-twitter.png" alt="">
                <img src="/img/footer-youtube.png" alt="">
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
footer {
    background-color: #303030;
}

.row {
    height: 100px;
    display: flex;
}

.col {
    flex-basis: calc(100% / 2);
    display: flex;
    justify-content: center;
    align-items: center;
}

h4 {
    color: white;
    padding: 10px;
    border: 2px solid #0281f7;
}

h3 {
    color: #265ecd;
    margin-right: 10px;
}

img {
    margin: 0 10px;
}
</style>