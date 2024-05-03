<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppBlueBarr from './components/AppBlueBarr.vue';
import AppListSite from './components/AppListSite.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  components: {
    AppHeader,
    AppMain,
    AppBlueBarr,
    AppListSite,
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
  <AppListSite />
  <AppFooter />
</template>

<style lang="scss">

</style>