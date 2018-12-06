<template>
  <div>

    <!-- AboveNavbar -->
    <above-nav-bar/>

    <!-- Navbar -->
    <navbar/>

    <!-- Header -->
    <custom-header/>

    <!-- Achievements -->
    <achievements/>

  </div>
</template>

<script>
import AboveNavBar from './../components/AboveNavBar'
import Navbar from './../components/Navbar'
import CustomHeader from './../components/Header'
import Achievements from './../components/Achievements'

export default {
  name: 'HomePage',
  components: {
    AboveNavBar,
    Navbar,
    CustomHeader,
    Achievements,
  },
  data () {
    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
body {
  scroll-behavior: smooth;
}
</style>
