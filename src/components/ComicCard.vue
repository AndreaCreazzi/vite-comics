<script>
export default {
    props: {
        heroes: Array
    },
    data() {
        return
    }
}
</script>

<template>
    <div v-for="hero in heroes" class="card">
        <div class="img-container">
            <img :src="hero.thumb" alt="">
        </div>
        <p>{{ hero.series }}</p>
    </div>
</template>

<style lang="scss" scoped>
.card {
    flex-basis: calc(100% / 6);
    display: flex;
    flex-direction: column;
    margin-top: 40px;
    padding: 0 30px;

    .img-container {
        width: 100%;
        height: 200px;
        overflow: hidden;
    }

    img {
        width: 100%;
        height: auto;
        display: block;
        cursor: pointer;
    }

    p {
        color: white;
        font-size: 0.8rem;
        display: block;
        text-align: center;
        text-transform: uppercase;
    }
}
</style>