<script>

export default {
    data () {
        return {

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
                <li><a href="">CHARACTERS</a></li>
                <li><a href="">COMICS</a></li>
                <li><a href="">MOVIES</a></li>
                <li><a href="">TV</a></li>
                <li><a href="">GAMES</a></li>
                <li><a href="">COLLECTIBLES</a></li>
                <li><a href="">VIDEOS</a></li>
                <li><a href="">FANS</a></li>
                <li><a href="">NEWS</a></li>
                <li><a href="">SHOP</a></li>
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
    width: 40%;
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
              text-decoration: none;
              font-size: .7rem;
              color: $text-nav-bar-color;
              cursor: pointer;
           }
     }
   }

}

</style>