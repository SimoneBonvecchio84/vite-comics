<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppBlueBarr from './components/AppBlueBarr.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  components: {
    AppHeader,
    AppMain,
    AppBlueBarr,
    AppFooter  
  },

  data () {
    return {

    }
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppBlueBarr />
  <AppFooter />
</template>

<style lang="scss">

</style>