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
        <img :src="hero.thumb" alt="">
        <p>{{ hero.series }}</p>
    </div>
</template>

<style lang="scss" scoped>
.card {
    flex-basis: calc(100% / 6);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    img {
        max-width: 130px;
        height: auto;
        display: block;
        margin-bottom: 10px;
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