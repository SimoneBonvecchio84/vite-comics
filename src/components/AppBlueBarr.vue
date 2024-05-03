<script>
export default {
    data () {
        return {
            inconsList: [
                {
                    icon: "buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS"

                },
                {
                    icon: "buy-comics-merchandise.png",
                    text: "DC MERCHANDISE"

                },
                {
                    icon: "buy-comics-shop-locator.png",
                    text: "SUBSCRIPTION"
                    
                },
                {
                    icon: "buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR"

                },
                {
                    icon: "buy-dc-power-visa.svg",
                    text: "DC POWER VISA"

                },
            ]
        }
    },
    methods: {
        getIconsUrl (iconName) {
            return new URL(`../assets/img/${iconName}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <section>
        <div class="general-container">
            <ul>
                <li>
                    <img v-for="curIcon in inconsList" :src="getIconsUrl(curIcon.icon)" alt="">
                </li>
            </ul>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;

section {
    background-color: $primary-color;
    padding: 3rem 0;
    color: white;
}
</style>