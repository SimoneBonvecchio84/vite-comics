<script>
export default {
    data () {
        return {
            dcComicsList:[
                "Charracters", "Comics", "Movies", "TV", "Games", "Videos", "News"
            ],
            shopList: [
                "Shop DC", "Shop DC Collectibles", 
            ],
            dcList: [
                "Terms Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", 
                "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"
            ],
            sitesList: [
                "DC", "MAD Magazine", "DC kids", "DC Universe", "DC Power Visa"
            ]
        }
    }
}
</script>

<template>
 <section>
    <div class="general-container">
        
        <div class="container-list">
            <ul>
                <h4>DC COMICS</h4>
                <li v-for="curDcComics in dcComicsList"><a href=""> {{ curDcComics }}</a></li>
            </ul>
            <ul>
                <h4>SHOP</h4>
                <li v-for="curShop in shopList"><a href="">{{ curShop }}</a></li>
            </ul>    
            <ul>
                <h4>DC</h4>
                <li v-for="curDcList in dcList"><a href=""> {{ curDcList }}</a></li>
            </ul>
            <ul>
                <h4>SITES</h4>
                <li v-for="curSites in sitesList"><a href="">{{ curSites }}</a></li>
            </ul>
        </div>
        
      
        
        <div class="container-logo">
          

        </div>
    </div>
 </section>
</template>

<style scoped leng="scss">


section {   
   background-image: url(../assets/img/footer-bg.jpg);
   background-repeat: no-repeat;
   background-size: cover;
   
   
   
}

.general-container {
    display: flex;
    justify-content: space-between;
    
    .container-list {
        width: 30%;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        padding:  1rem 0;
        height: 250px;
        row-gap: 1rem;
        column-gap: 1.5rem;
       
        h4 {
            color: white;
            font-size: .8rem;
        }
        ul {
            list-style-type: none;
            
            a {
                color:rgb(122, 119, 119) ;
                text-decoration: none;
                font-size: .6rem;
                font-weight: 600;
            }
        }
    }
    
    .container-logo {
        width: 40%;
        background-image: url(../assets/img/dc-logo-bg.png); 
        background-position: center; 
        background-size:cover;
 }

} 
</style>