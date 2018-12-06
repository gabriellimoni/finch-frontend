<template lang="html">
  <div id="clients" class="section has-background-link">

    <!-- header -->
    <clients-header/>

    <!-- list -->
    <clients-list/>

  </div>
</template>

<script>
import ClientsHeader from './ClientsHeader'
import ClientsList from './ClientsList'

export default {
  components: {
    ClientsHeader,
    ClientsList,
  }
}
</script>

<style lang="css">
</style>
