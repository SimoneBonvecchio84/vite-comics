<script>
export default {
   props: {
    cardImage  : String,
    cardSeries : String,
   }
}
</script>

<template>
    <div class="card">
        <img :src="cardImage" :alt="cardSeries">
        <h4>{{ cardSeries }}</h4>
    </div>

</template>

<style scoped lang="scss">
    img {
       max-width: 100%;
       height: 170px;
    }

    h4 {
        color: white;
        font-size: .7rem;
        margin-top: .5rem;
    }
</style>