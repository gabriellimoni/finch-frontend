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

    <!-- clients -->
    <clients/>

    <!-- services -->
    <services/>

    <!-- Testimonial -->
    <testimonial/>

  </div>
</template>

<script>
import AboveNavBar from './../components/AboveNavBar'
import Navbar from './../components/Navbar'
import CustomHeader from './../components/Header'
import Achievements from './../components/Achievements'
import Clients from './../components/Clients'
import Services from './../components/Services'
import Testimonial from './../components/Testimonial'

export default {
  name: 'HomePage',
  components: {
    AboveNavBar,
    Navbar,
    CustomHeader,
    Achievements,
    Clients,
    Services,
    Testimonial,
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
