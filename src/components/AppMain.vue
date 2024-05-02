<script>

export default {
    data () {
        return {

        }
    }
}

</script>

<template>
    
    <main>
        <section class="goesHear-container">
            
            <div class="cont">
                <h3>  -->Content goes here<-- </h3>
            </div>

        </section>
    </main>
    
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;
 .goesHear-container {
    background-color: $black-color;
    height: 100px;
    display: flex;
    @include flex(row,center,center);
    
    .cont{
        width: 70%;
        
        h3 {
            color: white;
        }
        
    }
 
}

</style>