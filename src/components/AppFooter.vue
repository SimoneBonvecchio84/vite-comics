<script>

export default {
    data () {
        return {
            listIcons: [
               "footer-facebook.png",
               "footer-twitter.png",
               "footer-youtube.png",
               "footer-pinterest.png",
               "footer-periscope.png"
            ]
        }
    },
    methods: {
        getIcon (iconName) {
            return new URL(`../assets/img/${iconName}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <section>
       <div class="general-container">
        
        <div class="container-btn">
           
            <button><a href="">SING-UP NOW!</a></button>

        </div>

        <div class="container-link">
            <h4>FOLLOW US</h4>
            <ul>
                <li v-for="curIcons in listIcons">
                    <a href="">
                        <img :src="getIcon(curIcons)" alt="">
                    </a>
                </li>
            </ul>
        </div>
       
    </div> 
    </section>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;
    section{
        background-color:rgb(48 48 48);
        
        .general-container {
            display: flex;
            justify-content: space-between;
            padding: 2rem 0;

            .container-btn{
                
            }

            .container-link {
                display: flex;
                align-items: center;
                column-gap: 1rem;
                h4 {
                    color: $primary-color;
                    font-size: .7rem;
                }

                ul {
                    display: flex;
                    list-style-type: none;
                    img {
                        width: 50%;
                    }
                }
            }
        }
    }
</style>