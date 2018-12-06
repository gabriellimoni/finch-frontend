<template lang="html">
  <div id="services" class="section has-text-centered">
    <!-- util-header -->
    <util-header title="Our Services" subtitle="With Passion & Experience"/>

    <!-- ServicesList -->
    <services-list/>

  </div>
</template>

<script>
import UtilHeader from './../utils/UtilHeader'
import ServicesList from './ServicesList'

export default {
  components: {
    UtilHeader,
    ServicesList,
  }
}
</script>

<style lang="css">
</style>
