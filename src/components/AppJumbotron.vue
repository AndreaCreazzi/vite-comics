<script>
export default {
    data() {
        return {
            images: [
                {
                    url: "img/buy-comics-digital-comics.png",
                    Text: "DIGITAL COMICS"
                },
                {
                    url: "img/buy-comics-merchandise.png",
                    Text: "DC MERCHANDISE"
                },
                {
                    url: "img/buy-comics-shop-locator.png",
                    Text: "SUBSCRITION"
                },
                {
                    url: "img/buy-comics-subscriptions.png",
                    Text: "COMIC SHOP LOCATOR"
                },
                {
                    url: "img/buy-dc-power-visa.svg",
                    Text: "DC POWER VISA"
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <figure>
            <p v-for="image in images"><img :src="image.url" alt="">{{ image.Text }}</p>
        </figure>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: #0282f9;
}

img {
    max-width: 60px;
    height: 60px;
    margin-right: 20px;
}

figure {
    height: 171px;
    display: flex;
    justify-content: center;
    align-items: center;
}

p {
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 20px;
}
</style>