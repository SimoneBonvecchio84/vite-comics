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
                <li v-for="curIcon in inconsList" >
                    <img :src="getIconsUrl(curIcon.icon)" alt="">
                    <h4> {{ curIcon.text }}</h4>
                </li>
            </ul>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;
@use "../style/partials/mixin" as *;
section {
    background-color: $primary-color;
    padding: 3rem 0;
    color: white;


    ul {
        list-style-type: none;
        display: flex;
        justify-content: space-evenly;

        li {
            display: flex;
            align-items: center;
            gap: 1rem;
            img {
                height: 50px;
            }

            h4 {
                font-size: .7rem;
                font-weight: 300;
            }

        }
    }
}
</style>