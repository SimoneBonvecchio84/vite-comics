<script>

export default {
    data () {
        return {
            menu: [
                {
                    title: "CHARACTERS",
                    isActive: false
                },
                {
                    title: "COMICS",
                    isActive: true
                },
                {
                    title: "MOVIE",
                    isActive: false
                },
                {
                    title: "TV",
                    isActive: false
                },
                {
                    title: "GAMES",
                    isActive: false
                },
                {
                    title: "COLLECTIBLES",
                    isActive: false
                },
                {
                    title: "VIDEOS",
                    isActive: false
                },
                {
                    title: "FANS",
                    isActive: false
                },
                {
                    title: "NEWS",
                    isActive: false
                },
                {
                    title: "SHOP",
                    isActive: false
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="header-logo">
            <img src="../assets/img/dc-logo.png" alt="logo della dc comics">
        </div>

        <div class="header-nav">
            <ul class="navigation">
                <li v-for="curNav in menu" >
                    <a :class="{'active': curNav.isActive }" href=""> {{ curNav.title}} </a>
                </li>
                
            </ul>
        </div>
    </header>
</template>

<style  lang="scss" scoped>
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;
header {
   margin-top:50px ;
   display: flex;

   .header-logo {
    width: 30%;
    text-align: center;

    img {
        width: 15%;
    }
   }

   .header-nav {
     display: flex;
       .navigation {
           @include flex(row,center,center);
           list-style-type: none; 
           gap: 1rem; 
               
           a {
              padding: 10px ;
              text-decoration: none;
              font-size: .7rem;
              color: $text-nav-bar-color;
              cursor: pointer;

              &:hover {
                color: $primary-color;
              };

              &.active {
                background-color: $primary-color;
                color: white;
                
              }
           }
     }
   }

}

</style>