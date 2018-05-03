<template>
  <div id="app">
    <topsocial/>
    <navigation/>
    <router-view/>
    <!-- <cfooter/> -->
  </div>
</template>

<script>
import navigation from './components/Nav';
import topsocial from './components/TopSocial'

export default {
  name: 'App',
  components: {
    navigation,
    topsocial,
  }
}
</script>

<style lang="sass">
  * 
    font-family: 'Raleway', 'Helvetica', Arial, sans-serif
    // overflow-x: hidden

</style>
